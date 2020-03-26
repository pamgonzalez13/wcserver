<template>
<nav class="navbar navbar-expand-lg navbar-light bg-light" style="background: #2d3246;">
  <a class="navbar-brand " href="#" style="text-shadow: 1px 1px #000000;"><strong>WCSERVER</strong></a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mx-auto">
      <router-link class="spacing" v-for="routes in links" 
      v-bind:key="routes.id"
      :to="`${routes.page}`">{{routes.text}}</router-link>
    </ul>
  </div>
</nav>
</template>
<script>
export default {
  name: 'Navigation',
  data() {
    return {
      links: [
        {
          id: 0,
          text: 'Home',
          page:'/'
        },
        {
          id: 1,
          text: 'Members',
          page:'/Members'
        },
        {
          id: 2,
          text: 'News',
          page:'/News'
        }
      ]
    }
  }
}
</script>

<style> 
  .spacing { 
    Margin-right: 10px; 
    text-decoration: none;
    color: #000000;
    font-size: 18px;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: 2px;
    padding-left: 30px;
    text-shadow: 1px 1px #000000;
  } 
  .spacing a{
    text-decoration: none;
    color: #fff;
    font-size: 25px;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: 2px;
  }
</style>
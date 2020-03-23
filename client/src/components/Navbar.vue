<template>
<nav class="navbar navbar-expand-lg navbar-light" style="background: #2d3246;">
  <a class="navbar-brand" href="#">SERVER NEWS</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <router-link class="spacing" v-for="routes in links" 
      v-bind:key="routes.id"
      :to="`${routes.page}`">{{routes.text}}</router-link>
    </ul>
    <form class="form-inline my-2 my-lg-0">
      <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
    </form>
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
    color: #fff;
    font-size: 18px;
    text-transform: uppercase;
    font-weight: bold;
    letter-spacing: 2px;
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
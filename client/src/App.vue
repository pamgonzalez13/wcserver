<template>
  <div>
    <Navigation></Navigation>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script src="//maxcdn.bootstrapcdn.com/bootstrap/4.1.1/js/bootstrap.min.js"></script>
<script src="//cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>

<script>
import Navigation from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'app',
  components: {
    'Navigation': Navigation,
    'Footer' : Footer
  }
}
</script>

<style>
body{
background: url(https://image.shutterstock.com/image-vector/internet-connection-abstract-sense-science-260nw-554257006.jpg) !important;
background-repeat: no-repeat !important;
background-size: cover !important;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-bottom: 10px;
}


#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  padding: 20px;
}

#nav a.router-link-exact-active {
  color: skyblue;
}
</style>

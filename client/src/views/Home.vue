<template>
<div>
<div class="slider">
    <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
      <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
      <li data-target="#carouselExampleCaptions" data-slide-to="1"></li>
      <li data-target="#carouselExampleCaptions" data-slide-to="2"></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/update.jpg" class="d-block w-100 " alt="...">
        <div class="carousel-caption d-none d-md-block text-dark" style="width: auto;">
          <h3>NEWS</h3>
          <p>COVID-19 Pandemic Update 2020!</p>
          <button class="btn btn-outline-dark my-2 my-sm-0 bg-light"><a class="text-decoration-none text-dark" href="#">Learn More</a></button>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/update.jpg" class="d-block w-100 " alt="...">
        <div class="carousel-caption d-none d-md-block" style="width: auto;">
          <h3>PRODUCTS</h3>
          <p>Ryzen has new released processor.</p>
          <button class="btn btn-outline-dark my-2 my-sm-0 bg-light"><a class="text-decoration-none text-dark" href="#">Learn More</a></button>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/banner1.jpg" class="d-block w-100 " alt="...">
        <div class="carousel-caption d-none d-md-block " style="width: auto;">
          <h3>DEVELOPER</h3>
          <p>What will be the next innovation.</p>
          <button class="btn btn-outline-dark my-2 my-sm-0 bg-light"><a class="text-decoration-none text-dark" href="#">Learn More</a></button>
        </div>
      </div>
    </div>
    <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>
</div>
</div>
</template>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script> 
<script>
export default {
  name: 'Home',

}
</script>

<style>
body{
  background: #000000;
}

.carousel-inner p {
  font-size: 20px !important;
  font-weight: bolder !important;
}

@keyframes loader{
  0%{
    transform: scale(0);
  }
  50%{
    opacity: 1;
  }
  100%{
    transform: scale(1);
    opacity: 0;
  }
}

.carousel-item{
    height: 100vh;
    min-height: 300px;
    background: no-repeat center center scroll;
    -webkit-background-size:cover;
    background-size: cover;
  }

  .carousel-caption{
    bottom: 370px;
  }

  .carousel-caption h3{
    font-size: 45px;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-top: 25px;
  }

 .carousel-caption p{
  width: 75%;
  margin: auto;
  font-size: 18px;
  line-height: 1.9;
  }

  .navbar-light .navbar-brand{
    color: #fff;
    font-size: 25px;
    text-transform: uppercase;
    font-weight: bold;
    ;letter-spacing: 2px;
  }

  .nav-link{
    font-weight: bold;
    letter-spacing: 2px;
  }

.navbar-light .navbar-toggler{
  background: #fff;
}
</style>
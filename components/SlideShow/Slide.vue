<template>
  <no-ssr class="container">
    <agile  
    :arrows="false" :speed="750"
    :timing="'linear'" :fade="true"
    :dots="false"
    :autoplay="true" :pauseOnHover="false">
      <div class="slide slide--1">
      </div>
      <div class="slide slide--2">
      </div>
      <div class="slide slide--3">
      </div>
    </agile>
  </no-ssr>
</template>
<style scoped>
.container {
  width: 75%;
  height: 600px;
  margin-top: 60px;
}
.slide {
  margin:30px auto;
  width: 100%;
  height: 600px;
  background-size: cover;
  background-repeat: no-repeat;
}
.slide--1 {
  background-image: url("https://www.sharda.ac.in/blog/wp-content/uploads/2017/08/4-Main-Types-of-Law-Which-One-Is-the-Best-For-You-1024x538.jpg");
}
.slide--2 {
  background-image: url("https://cdn-images-1.medium.com/max/2000/1*PwXaZrVqmx1pgN3IhwbXfQ.jpeg");
}
.slide--3 {
  background-image: url("https://s-i.huffpost.com/gen/1720141/images/o-LAW-facebook.jpg");
}
</style>

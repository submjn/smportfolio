<template>
    <carousel>
        <carousel-item>
        <h2>#1</h2>
        <img src="https://octodex.github.com/images/original.png" alt="">
        </carousel-item>
        <carousel-item>
        <h2>#2</h2>
        <img src="https://octodex.github.com/images/octobiwan.jpg" alt="">
        </carousel-item>
        <carousel-item>
        <h2>#3</h2>
        <img src="https://octodex.github.com/images/daftpunktocat-thomas.gif" alt="">
        </carousel-item>
        <carousel-item>
        <h2>#4</h2>
        <img src="https://octodex.github.com/images/adventure-cat.png" alt="">
        </carousel-item>
    </carousel>
</template>

<style>
#smCarousel {
  margin: 10px auto;
  width: 80%;
}

.carousel-component {
  position: relative;
  overflow: hidden;
}

.carousel-page {
  visibility: hidden;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  transition: 0.5s;
  padding: 10px;
  border: 1px solid #EEE;
}

.carousel-page h2 {
margin: 0;
}

.carousel-page   img {
width: 300px;
}

.carousel-page.active {
  visibility: visible;
  position: static;
}

.carousel-nav-prev,
.carousel-nav-next {
  position: absolute;
  top: 50%;
  transform: translate(0, -50%);
  display: block;
  width: 50px;
  height: 50px;
  border: 0;
  background: rgba(0, 0, 0, 0.5);
  color: #FFF;
  cursor: pointer;
}

.carousel-nav-prev {
  left: 5px;
}

.carousel-nav-next {
  right: 5px;
}

</style>

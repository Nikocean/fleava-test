<template>
  <div id="banners">
    <!-- <div class="banner one">
      <h1>Banner One</h1>
      <div class="image"></div>
    </div>
    <div class="banner two">
      <h1>Second Banner</h1>
      <div class="image"></div>
    </div>
    <div class="banner three">
      <h1>Banner <span>The Third</span></h1>
      <div class="image"></div>
    </div> -->
    <!-- <div class="carousel" data-carousel>
      <button class="carousel-button prev" data-carousel-button="prev">&#8656;</button>
      <button class="carousel-button next" data-carousel-button="next">&#8658;</button>
      <ul data-slides>
        <li class="slide" data-active>
          <img src="https://source.unsplash.com/78A265wPiO4" alt="Nature Image #1">
        </li>
        <li class="slide">
          <img src="https://source.unsplash.com/eOpewngf68w" alt="Nature Image #2">
        </li>
        <li class="slide">
          <img src="https://source.unsplash.com/ndN00KmbJ1c" alt="Nature Image #3">
        </li>
      </ul>
    </div> -->
    <div class="slider">
      <div class="slides">
        <!--radio buttons start-->
        <input type="radio" name="radio-btn" id="radio1">
        <input type="radio" name="radio-btn" id="radio2">
        <input type="radio" name="radio-btn" id="radio3">
        <input type="radio" name="radio-btn" id="radio4">
        <!--radio buttons end-->
        <!--slide images start-->
        <div class="slide first">
          <img src="../img/0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg" alt="">
        </div>
        <div class="slide">
          <img src="../img/ff642f58-71fc-4cee-9d91-d525b1c641d2.jpg" alt="">
        </div>
        <div class="slide">
          <img src="../img/e5740d7a-73ce-4643-8761-2f59c29a40f9.jpg" alt="">
        </div>
        <div class="slide">
          <img src="../img/097470ab-7879-493e-bc98-5dc4fd09cb54.jpg" alt="">
        </div>
        <!--slide images end-->
        <!--automatic navigation start-->
        <div class="navigation-auto">
          <div class="auto-btn1"></div>
          <div class="auto-btn2"></div>
          <div class="auto-btn3"></div>
          <div class="auto-btn4"></div>
        </div>
        <!--automatic navigation end-->
      </div>
      <!--manual navigation start-->
      <div class="navigation-manual">
        <label for="radio1" class="manual-btn"></label>
        <label for="radio2" class="manual-btn"></label>
        <label for="radio3" class="manual-btn"></label>
        <label for="radio4" class="manual-btn"></label>
      </div>
      <!--manual navigation end-->
    </div>
  </div>
</template>

<style scoped>
/* #banners {
  height: 10rem;
  overflow-x: hidden;
  position: relative;
  width: 100%;
}
#banners .banner {
  animation: bannerOne 15s linear infinite;
  height: 10rem;
  position: absolute;
  width: 100%;
}
#banners .banner.one h1,
#banners .banner.two h1,
#banners .banner.three h1 {
  color: #fff;
  font-size: 2rem;
  padding: 1rem;
  margin: 0;
}
#banners .banner.one h1 span,
#banners .banner.two h1 span,
#banners .banner.three h1 span {
  display: block;
}
#banners .banner.one .image,
#banners .banner.two .image,
#banners .banner.three .image {
  height: 100%;
  position: absolute;
  top: 0;
  width: 50%;
}
#banners .banner.one {
  background: red;
}
#banners .banner.one h1 {
  text-align: right;
  width: 50%;
}
#banners .banner.one .image {
  background: url('http://placehold.it/400x400') no-repeat right center;
  background-size: 100%;
  right: 0;
}
#banners .banner.two {
  animation-name: bannerTwo;
  background: blue;
}
#banners .banner.two h1 {
  text-align: center;
}
#banners .banner.two .image {
  background: url('http://placehold.it/1000x200') no-repeat center bottom;
  background-size: 100%;
  top: 50%;
  height: 50%;
  width: 100%;
}
#banners .banner.three {
  animation-name: bannerThree;
  background: green;
}
#banners .banner.three h1 {
  float: right;
  width: 50%;
}
#banners .banner.three .image {
  background: url('http://placehold.it/400x400') no-repeat left center;
  background-size: 100%;
  left: 0;
}
@keyframes bannerOne {
  0% {
    left: 0;
  }
  31% {
    left: 0;
  }
  34% {
    left: -100%;
  }
  97% {
    left: 100%;
  }
  100% {
    left: 0;
  }
}
@keyframes bannerTwo {
  0% {
    left: 100%;
  }
  31% {
    left: 100%;
  }
  34% {
    left: 0;
  }
  64% {
    left: 0;
  }
  67% {
    left: -100%;
  }
  100% {
    left: -100%;
  }
}
@keyframes bannerThree {
  0% {
    left: 100%;
  }
  64% {
    left: 100%;
  }
  67% {
    left: 0;
  }
  97% {
    left: 0;
  }
  100% {
    left: -100%;
  }
}

@media (min-width: 321px) and (max-width: 728px) {
  #banners {
    height: 12rem;
  }
  #banners .banner.one,
  #banners .banner.two,
  #banners .banner.three {
    height: 12rem;
  }
  #banners .banner.one h1,
  #banners .banner.two h1,
  #banners .banner.three h1 {
    font-size: 3rem;
    padding: 1.5rem;
  }
}

@media (min-width: 729px) and (max-width: 960px) {
  #banners {
    height: 20rem;
  }
  #banners .banner.one,
  #banners .banner.two,
  #banners .banner.three {
    height: 20rem;
  }
  #banners .banner.one h1,
  #banners .banner.two h1,
  #banners .banner.three h1 {
    font-size: 6rem;
    padding: 2rem;
  }
}

@media (min-width: 961px) {
  #banners {
    height: 20rem;
  }
  #banners .banner.one,
  #banners .banner.two,
  #banners .banner.three {
    height: 20rem;
  }
  #banners .banner.one h1,
  #banners .banner.two h1,
  #banners .banner.three h1 {
    font-size: 6rem;
    padding: 2rem;
  }
} */

/* *, *::before, *::after {
  box-sizing: border-box;
}

body {
  margin: 0;
}

.carousel {
  width: 100vw;
  height: 100vh;
  position: relative;
}

.carousel > ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.slide {
  position: absolute;
  inset: 0;
  opacity: 0;
  transition: 200ms opacity ease-in-out;
  transition-delay: 200ms;
}

.slide > img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
}

.slide[data-active] {
  opacity: 1;
  z-index: 1;
  transition-delay: 0ms;
}

.carousel-button {
  position: absolute;
  z-index: 2;
  background: none;
  border: none;
  font-size: 4rem;
  top: 50%;
  transform: translateY(-50%);
  color: rgba(255, 255, 255, .5);
  cursor: pointer;
  border-radius: .25rem;
  padding: 0 .5rem;
  background-color: rgba(0, 0, 0, .1);
}

.carousel-button:hover,
.carousel-button:focus {
  color: white;
  background-color: rgba(0, 0, 0, .2);
}

.carousel-button:focus {
  outline: 1px solid black;
}

.carousel-button.prev {
  left: 1rem;
}

.carousel-button.next {
  right: 1rem;
} */

#banners{
  margin: 0;
  padding: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.slider{
  width: 800px;
  height: 500px;
  overflow: hidden;
}

.slides{
  width: 500%;
  height: 500px;
  display: flex;
}

.slides input{
  display: none;
}

.slide{
  width: 20%;
  transition: 2s;
}

.slide img{
  width: 800px;
  height: 500px;
}

/*css for manual slide navigation*/

.navigation-manual{
  position: absolute;
  width: 800px;
  margin-top: -40px;
  display: flex;
  justify-content: center;
}

.manual-btn{
  border: 2px solid rgb(95, 92, 104);
  padding: 5px;
  border-radius: 10px;
  cursor: pointer;
  transition: 1s;
}

.manual-btn:not(:last-child){
  margin-right: 40px;
}

.manual-btn:hover{
  background: rgb(255, 255, 255);
}

#radio1:checked ~ .first{
  margin-left: 0;
}

#radio2:checked ~ .first{
  margin-left: -20%;
}

#radio3:checked ~ .first{
  margin-left: -40%;
}

#radio4:checked ~ .first{
  margin-left: -60%;
}

/*css for automatic navigation*/

.navigation-auto{
  position: relative;
  display: flex;
  width: 800px;
  justify-content: center;
  margin-top: 460px;
}

.navigation-auto div{
  border: 2px solid #40D3DC;
  padding: 5px;
  border-radius: 10px;
  transition: 1s;
}

.navigation-auto div:not(:last-child){
  margin-right: 40px;
}

#radio1:checked ~ .navigation-auto .auto-btn1{
  background: #40D3DC;
}

#radio2:checked ~ .navigation-auto .auto-btn2{
  background: #40D3DC;
}

#radio3:checked ~ .navigation-auto .auto-btn3{
  background: #40D3DC;
}

#radio4:checked ~ .navigation-auto .auto-btn4{
  background: #40D3DC;
}
</style>

<script>
// const buttons = document.querySelectorAll("[data-carousel-button]")

// buttons.forEach(button => {
//   button.addEventListener("click", () => {
//     const offset = button.dataset.carouselButton === "next" ? 1 : -1
//     const slides = button
//       .closest("[data-carousel]")
//       .querySelector("[data-slides]")

//     const activeSlide = slides.querySelector("[data-active]")
//     let newIndex = [...slides.children].indexOf(activeSlide) + offset
//     if (newIndex < 0) newIndex = slides.children.length - 1
//     if (newIndex >= slides.children.length) newIndex = 0

//     slides.children[newIndex].dataset.active = true
//     delete activeSlide.dataset.active
//   })
// })

    var counter = 1;
    setInterval(function(){
      document.getElementById('radio' + counter).checked = true;
      counter++;
      if(counter > 4){
        counter = 1;
      }
    }, 5000);
</script>

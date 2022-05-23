<template>
  <div class="block">
    <!-- <img src="../img/a109df5.png" alt="" class="img-bg"> -->
    <img
      src="../img/0a92d769-ae4f-4a86-b5d6-67fbb4bc4472.jpg"
      data-speed="-1"
      class="img-parallax animate fadeInLeft"
    />

    <div class="resort">
      <div class="container">
        <p class="resort-title animate fadeInUp">
          The <br />
          Resort
        </p>
        <p class="resort-desc">
          Jannata Resort & Spa is a boutique property with tranquil valley views
          in the rural village of Sebali, just outside of Ubud.
          <br />
          <br />
          It is attuned to the surrounding environment through a thoughtful
          design that respects Bali’s rich artistry and cultural heritage.
        </p>
        <p class="resort-link animate fadeInUp">READ THE STORY</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.block {
  background: #f0f0f5;
  padding: 150px 0 100px 300px;
  position: relative;
  z-index: -2;
}

/* .block .img-bg{
    height: 100%;
  width: 250px;
  left: -25%;
  position: relative;
} */

.block .img-parallax {
  position: absolute;
  width: 520px;
  height: 625px;
  z-index: 1;
  -webkit-animation-delay: 2.5s;
  -moz-animation-delay: 2.5s;
  animation-delay: 2.5s;
}

.resort {
  padding: 50px 60px 70px;
  width: 900px;
  height: 560px;
  background: #ffff;
  margin: 5rem 0 0 10rem;
}

.resort .container {
  position: relative;
  left: 45%;
  width: 300px;
}

.resort .resort-desc {
  max-width: 300px;
  font-family: 'Open Sans', sans-serif;
  font-size: 12px;
  font-weight: 400;
  color: rgb(95, 92, 104);
  word-spacing: 1px;
}

.resort .resort-title {
  -webkit-animation-delay: 0.5s;
  -moz-animation-delay: 0.5s;
  animation-delay: 0.5s;
  font-family: 'Playfair Display', serif;
  font-size: 59px;
  color: rgb(95, 92, 104);
  letter-spacing: 5px;
}

.resort .resort-link {
  color: rgb(103, 147, 52);
  font-weight: 400;
  font-size: 15px;
  letter-spacing: 1px;
  font-family: 'Open Sans', sans-serif;
  margin-top: 45px;
}

.resort-link:after {
  content: '';
  position: absolute;
  width: 100%;
  transform: scaleX(0);
  height: 2px;
  bottom: 0;
  left: 0;
  transform-origin: bottom right;
  transition: transform 0.25s ease-out;
}

.resort-link:hover:after {
  transform: scaleX(1);
  transform-origin: bottom left;
}

.animate {
  -webkit-animation-duration: 1s;
  animation-duration: 1s;
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
}

@-webkit-keyframes fadeInUp {
  from {
    opacity: 0;
    -webkit-transform: translate3d(0, 100%, 0);
    transform: translate3d(0, 100%, 0);
  }

  to {
    opacity: 1;
    -webkit-transform: none;
    transform: none;
  }
}
@keyframes fadeInUp {
  from {
    opacity: 0;
    -webkit-transform: translate3d(0, 100%, 0);
    transform: translate3d(0, 100%, 0);
  }

  to {
    opacity: 1;
    -webkit-transform: none;
    transform: none;
  }
}

.fadeInUp {
  -webkit-animation-name: fadeInUp;
  animation-name: fadeInUp;
}

@-webkit-keyframes fadeInLeft {
  from {
    opacity: 0;
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }

  to {
    opacity: 1;
    -webkit-transform: none;
    transform: none;
  }
}
@keyframes fadeInLeft {
  from {
    opacity: 0;
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
  }

  to {
    opacity: 1;
    -webkit-transform: none;
    transform: none;
  }
}

.fadeInLeft {
  -webkit-animation-name: fadeInLeft;
  animation-name: fadeInLeft;
}
</style>

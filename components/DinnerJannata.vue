<template>
  <div class="block">
    <!-- <div class="img">
      
  </div> -->
    <img
      src="../img/e061b86c-217c-4b9f-87ec-bc67b45db7a0.jpg"
      data-speed="-1"
      class="img-parallax animate fadeInLeft"
    />

    <div class="dinner">
      <div class="container">
        <p class="dinner-title animate fadeInUp">
          Dinner with <br />
          <span style="color: rgb(103, 147, 52)">Jannata</span>
        </p>
        <p class="dinner-desc">
          Amateras Restaurant at Jannata Resort & Spa serves an extensive menu
          of Western and Asian cuisine that is driven by quality ingredients.
          <br /><br />
          The restaurant is located next to the lobby and extends out onto an
          open terrace for an alfresco dining experience. It is elevated over
          the main swimming pool with tropical views of lush valley greenery in
          the distance.
        </p>
        <p class="dinner-link animate fadeInUp">READ MORE</p>
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
  color: rgb(95, 92, 104);
}

.block .img-parallax {
  position: absolute;
  width: 892px;
  height: 584px;
  z-index: -1;
  -webkit-animation-delay: 2.5s;
  -moz-animation-delay: 2.5s;
  animation-delay: 2.5s;
}

.dinner {
  padding: 50px 60px 70px;
  width: 536px;
  height: 560px;
  background: #ffff;
  margin: 5rem 0 0 31rem;
}

.dinner .dinner-desc {
  max-width: 300px;
  font-size: 12px;
  font-weight: 400;
  font-family: 'Open Sans', sans-serif;
  word-spacing: 1px;
}

.dinner .dinner-title {
  -webkit-animation-delay: 0.5s;
  -moz-animation-delay: 0.5s;
  animation-delay: 0.5s;
  font-size: 59px;
  font-weight: 400;
  font-family: 'Playfair Display', serif;
  letter-spacing: 3px;
}

.dinner .dinner-link {
  color: rgb(103, 147, 52);
  font-weight: 400;
  font-size: 15px;
  letter-spacing: 1px;
  font-family: 'Open Sans', sans-serif;
  margin-top: 45px;
}

.dinner-link:after {
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

.dinner-link:hover:after {
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

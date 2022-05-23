<template>
  <div class="reviewers">
    <img src="../img/a109df5.png" alt="">
    <h2 class="sentence">
      <div class="slidingHorizontal">
        <span>This hotel is just so beautiful and peaceful. The staff is
              amazing, very kind and competent, always with a smile on their
              face and always there for you. The room we were in was beautiful,
              clean, very big. The bathroom was to die for, and the view
              breathtaking.
              <p>— Sara B, Germany</p></span>
        <span>The resort excelled in all ways. The staff is super friendly
              &amp; helpful, the food is amazing (specially their Al carte
              breakfast), the room and infinity pool has fantastic views
              overlooking the rice paddy fields and the jungle.
              <p>— Nikita B, Australia</p></span>
        <span>I loved Jannata , i loved the people providing the service there,
              Always smiling always nice, they are so friendly that i really
              missed them during the rest of my trip and they made it harder for
              the other hotel staff to beat their friendly nice service.
              <p>— Michael S, Canada</p></span>
        <span>We could not thank all the staff at Jannata Resort and Spa
              enough! We stayed for 3 night at the end of October for our
              Honeymoon. We was upgraded to a pool villa for our stay and
              treated like royalty, Our private infinity pool was so beautiful
              and the views from our villa were breath taking!
              <p>— Laurenbull29, Germany</p></span>
      </div>
    </h2>
  </div>
</template>

<style scoped>
.reviewers{
  padding: 400px;
  background: #f0f0f5;
}
.reviewers h2{
  font-size: 20px;
  font-family: 'Playfair Display',serif;
  font-weight: lighter;
  word-spacing: 1px;
}
.reviewers img{
  height: 100%;
  width: 250px;
  /* margin-right: 600px; */
  left: -25%;
  position: relative;
}
.slidingHorizontal {
  display: inline;
  text-indent: 8px;
  margin-left: 200px;
  position: relative;
  bottom: 300px;
}
.slidingHorizontal span {
  animation: leftToRight 12.5s linear infinite 0s;
  -ms-animation: leftToRight 12.5s linear infinite 0s;
  -webkit-animation: leftToRight 12.5s linear infinite 0s;
  color: rgb(3, 3, 3);
  opacity: 0;
  overflow: hidden;
  position: absolute;
  width: 570px;
  height: 287px;
  text-align: center;
}

.slidingHorizontal span:nth-child(2) {
  animation-delay: 2.5s;
  -ms-animation-delay: 2.5s;
  -webkit-animation-delay: 2.5s;
}
.slidingHorizontal span:nth-child(3) {
  animation-delay: 5s;
  -ms-animation-delay: 5s;
  -webkit-animation-delay: 5s;
}
.slidingHorizontal span:nth-child(4) {
  animation-delay: 7.5s;
  -ms-animation-delay: 7.5s;
  -webkit-animation-delay: 7.5s;
}
.slidingHorizontal span:nth-child(5) {
  animation-delay: 10s;
  -ms-animation-delay: 10s;
  -webkit-animation-delay: 10s;
}

/*leftToRight Animation*/
@-moz-keyframes leftToRight {
  0% {
    opacity: 0;
  }
  5% {
    opacity: 0;
    -moz-transform: translateX(-50px);
  }
  10% {
    opacity: 1;
    -moz-transform: translateX(0px);
  }
  25% {
    opacity: 1;
    -moz-transform: translateX(0px);
  }
  30% {
    opacity: 0;
    -moz-transform: translateX(50px);
  }
  80% {
    opacity: 0;
  }
  100% {
    opacity: 0;
  }
}
@-webkit-keyframes leftToRight {
  0% {
    opacity: 0;
  }
  5% {
    opacity: 0;
    -webkit-transform: translateX(-50px);
  }
  10% {
    opacity: 1;
    -webkit-transform: translateX(0px);
  }
  25% {
    opacity: 1;
    -webkit-transform: translateX(0px);
  }
  30% {
    opacity: 0;
    -webkit-transform: translateX(50px);
  }
  80% {
    opacity: 0;
  }
  100% {
    opacity: 0;
  }
}
@-ms-keyframes leftToRight {
  0% {
    opacity: 0;
  }
  5% {
    opacity: 0;
    -ms-transform: translateX(-50px);
  }
  10% {
    opacity: 1;
    -ms-transform: translateX(0px);
  }
  25% {
    opacity: 1;
    -ms-transform: translateX(0px);
  }
  30% {
    opacity: 0;
    -ms-transform: translateX(50px);
  }
  80% {
    opacity: 0;
  }
  100% {
    opacity: 0;
  }
}
</style>

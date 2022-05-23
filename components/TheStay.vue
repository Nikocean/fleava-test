<template>
  <div class="the-stay">
    <div class="top">
      <img src="../img/a989adf.png" alt="" />
      <div class="stay">
        <h1 class="stay-title">THE STAY</h1>
        <p class="stay-desc animate fadeInUp">
          Stylish accommodation option at Jannata Resort & Spa incorporates a
          choice of 16 Deluxe Suites, 2 Deluxe Family Suite and 2 Pool Villas to
          anticipate all of your holiday needs. All categories are the epitome
          of Balinese luxury with customized interiors and essential home
          comforts.
          <br />
          <br />
          During pandemic, our resort has applied health protocols to ensure
          that our guests are safe. Before check-in, guests are encouraged to
          wash their hands and our team will check guests' body temperature.
          <br />
          <br />
          All the team members of Jannata Resort maintain the cleanliness in all
          areas including hotel rooms, restaurant, spa, kitchen. Every 4 hours
          disinfectant spray and physical distancing towards our pool decks,
          restaurant chairs, spa outlets are applied to ensure that our resort
          is in hygiene circumstance.
          <br />
          <br />
          Masks, face shields, hand sanitizer and also washing hands counter are
          fully prepared to welcome the new normal era ensuring all guests and
          staffs are safe and healthy.
          <br />
        </p>
      </div>
    </div>

    <div class="rooms">
      <div class="superior container">
        <img src="../img/DSCF4267_JPG.jpg" alt="" />
        <div class="overlay">
          <img src="../img/DSCF2425_JPG.jpg" alt="" class="img-overlay" />
        </div>
      </div>
      <br>
      <div class="pool container">
        <img src="../img/647A1103.jpg" alt="" />
        <div class="overlay">
          <img src="../img/DSCF2335_JPG.jpg" alt="" class="img-overlay2" />
        </div>
      </div>
      <br>
      <div class="deluxe container">
        <img src="../img/DSF0731-Edit-2_JPG.jpg" alt="" />
        <div class="overlay">
          <img src="../img/DSCF2390_JPG.jpg" alt="" class="img-overlay3" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.the-stay {
  background-color: rgb(95, 92, 104);
  padding: 150px 0;
}

.top {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.top img {
  height: 100%;
  width: 300px;
  object-fit: cover;
}

.top .stay {
  width: 496px;
  height: 462px;
  color: #fff;
}

.stay .stay-title {
  color: rgb(240, 240, 245);
  font-family: 'Playfair Display', serif;
  font-size: 35px;
  font-weight: 400;
  margin-bottom: 50px;
  letter-spacing: 1px;
}

.stay .stay-desc {
  color: rgb(216, 214, 226);
  font-family: 'Open Sans', sans-serif;
  font-weight: 400;
  font-size: 12px;
  word-spacing: 1px;
}

.rooms {
  position: relative;
}

.rooms img {
  width: 324px;
  height: 450px;
  object-fit: cover;
}

.rooms .pool{
  margin: 0 5px 0 5px;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  /* background-color: #008CBA; */
  overflow: hidden;
  width: 0;
  height: 100%;
  transition: 0.5s ease;
}

.container:hover .overlay {
  width: 100%;
}

.img-overlay {
  color: white;
  font-size: 20px;
  position: relative;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  white-space: nowrap;
}
.img-overlay2 {
  color: white;
  font-size: 20px;
  position: relative;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  white-space: nowrap;
}
.img-overlay3 {
  color: white;
  font-size: 20px;
  position: relative;
  top: 50%;
  left: 68.5%;
  -webkit-transform: translate(50%, 50%);
  -ms-transform: translate(0%, 50%);
  transform: translate(-50%, -50%);
  white-space: nowrap;
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
</style>

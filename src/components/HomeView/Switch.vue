<script setup>

import { RouterLink } from 'vue-router';

</script>

<template>

  <div class="bg">
    <div class="switch">
      <div class="switch1">
        <h2>Switching To SafeBank</h2>
        <p>Switching to us has never been easier! Stress free account switching done in minutes!</p>
        <button>
          <RouterLink to="signup" class="link">Apply</RouterLink>
        </button>
      </div>
      <div class="switch2">
        <img src="../../images/card.png" alt="">
      </div>
    </div>
    <div class="open">
      <div class="open1">
        <h2>Download The App!</h2>
        <p>Bank on the go with our SafeBank app! Travel and not have to worry about anything with our new mobile app. Takes just minutes to set up!</p>
        <button>Download</button>
      </div>
      <div class="open2">
        <img class="img" src="../../images/smartphone2.png" alt="">
      </div>
    </div>
  </div>
  
  

</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

.bg {
  background-color: rgb(250 250 249);
  padding-bottom: 20rem;
}

.switch {

  width: 90%;
  background-color: rgb(201, 199, 199);
  margin: 0 auto;
  border-radius: 24px;
  padding: 1rem 0;
  max-width: 600px;
}
.switch1 {
  padding-bottom: 2rem;
  padding-left: 1rem;
}
.switch h2 {
  margin-bottom: 8px;
}
.switch1 p {
  width: 90%;
}
.switch1 button {
  margin-top: 8px;
  width: 120px;
  height: 30px;
  border-radius: 12px;
  background-color: white;
  border: 1px solid blue;
}
.switch1 .link {
  text-decoration: none;
  font-size: 18px;
  color: blue;
}
.switch2 {
  text-align: center;
}
img {
  width: 200px;
}

.open {
  padding: 1rem 0;
  width: 90%;
  max-width: 740px;
  margin: 4rem auto 0;
  background-color: rgb(49 46 129);
  border-radius: 24px;
}
.open1 {
  padding-bottom: 2rem;
  padding-left: 1rem;
  color: white;
}
.open h2 {
  margin-bottom: 12px;
}
.open1 p {
  width: 80%;
}
.open button {
  width: 120px;
  height: 28px;
  margin-top: 1rem;
  border-radius: 12px;
  border: none;
}
.open2 {
  text-align: right;
}
.img {
  width: 280px;
}


@media only screen and (min-width: 700px){
  .switch {
    display: flex;
    align-items: center;
  }
  .switch div {
    width: 50%;
  }

  .open {
    display: flex;
    align-items: center;
  }
  .open p {
    width: 90%;
  }
}

</style>
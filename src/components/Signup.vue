<script setup>

import Header from './HomeView/Header.vue';

</script>

<template>

  <Header></Header>
  <div class="flex">
    <div class="side1">
      <img src="../images/growth.png" alt="">
      <p></p>
      <img class="img2" src="../images/sign-up.png" alt="">
    </div>
    <div class="side2">
      <h1>Create Account</h1>
      <p>Username</p>
      <input type="text">
      <p>Password</p>
      <input type="text">
    </div>
  </div>
  

</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

.flex {
  display: flex;
}
.side1 {
  height: 100vh;
  width: 50%;
  background-color: rgb(49 46 129);
  text-align: center;
  padding-top: 8rem;
}
.side1 img {
  width: 220px;
}
.side1 .img2 {
  width: 100px;
}
.side2 {
  height: 100vh;
  width: 50%;
  text-align: center;
  padding-top: 8rem;
}

.side2 input{
  width: 190px;
}

</style>
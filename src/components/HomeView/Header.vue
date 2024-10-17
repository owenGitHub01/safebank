<script setup>

import { RouterView, RouterLink } from 'vue-router';

</script>

<template>


<div class="main">
    <div class="width">

      <div class="title flex-title">

        <div class="flex-logo">
          <div class="bg">
            <img src="../../images/lock-variant.png" alt="">
          </div>
        </div>
        <h1>SafeBank</h1>
      </div>
      <div class="login-div">
        <button>
          <RouterLink class="link" to="/signin">Sign In</RouterLink>
        </button>
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
button {
  cursor: pointer;
}


.main {
  width: 100%;
  height: 70px;
  background-color: rgb(49 46 129);
}
.width {
  width: 90%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0 auto;
  padding-top: 8px;
}
.flex-logo {
  display: flex;
  align-items: center;
  padding-top: 4px;
}
.bg {
  background-color: white;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  background-color: rgb(129 140 248);
  margin-right: 4px;
}
img {
  width: 50px;
  height: 50px;
  
}

.flex-title {
  display: flex;
  align-items: center;
  color: white;
  width: 240px;
}

button {
  width: 100px;
  height: 30px;
  border-radius: 12px;
  background-color: aqua;
  border: none;
}
.link {
  text-decoration: none;
  color: black;
}

</style>

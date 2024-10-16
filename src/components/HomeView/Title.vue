<script setup>

import { RouterLink } from 'vue-router';

</script>

<template>

  <div class="main">
    <h1>Bank Smarter</h1>
    <h1 class="colour size">Bank Safer</h1>
    <h4 class="subheader">Banking With Confidence. Backed By Security</h4>
    <button>
      <RouterLink to="signup" class="link">Apply Now</RouterLink>
    </button>
    <div>
      <img class="review" src="../../images/safebank-trustpilot.png" alt="">
      <h2>Trust <span class="colour">Millions</span> Who Have Switched To SafeBank</h2>
    </div>
    
  </div>
  
  

</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

.main {
  height: 70vh;
  width: 100%;
  background-color: rgb(250 250 249);
  text-align: center;
  padding-top: 14rem;
}

.colour {
  color: rgb(49 46 129);
}
.size {
  font-size: 52px;
}
.subheader {
  padding: 2rem 0;
  width: 60%;
  margin: 0 auto;
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
  display: inline;
  width: 100%;
}

.review {
  width: 200px;
  display: inline;
}

.flex {
  display: flex;

}

</style>

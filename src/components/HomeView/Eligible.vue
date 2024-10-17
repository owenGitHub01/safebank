<script setup>

const eligible = [
  "Be 18+ years old",
  "Be a EU resident",
  "Have an EU mobile number",
]

</script>

<template>

<div class="main">
  <div class="cover">
    <h1>Are You Eligible To Use <span class="colour">SafeBank</span>?</h1>
  </div>
  <div class="rest">
    <div class="view">
      <div class="flex" v-for="item in eligible">
        <img class="icon" src="../../images/tick.png" alt="">
        <h2>{{ item }}</h2>
      </div>
    </div>
    <div class="image-div">
        <img class="image" src="../../images/smartphone.png" alt="">
    </div>
  </div>
  <h2 class="h2">So, What Are You Waiting For?</h2>
</div>

</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif; 
}

.main {
  background-color: rgb(250 250 249);
  padding-bottom: 20rem;
}

.cover {
  height: auto;
  padding-bottom: 1rem;
  width: 90%;
  max-width: 700px;
  margin: 0 auto;
  border-radius: 24px;
  background-color: rgb(103 232 249);
}
.cover h1 {
  padding: 20px 20px 0; 
}
.colour {
  color: blueviolet;
}

.rest {
  width: 90%;
  max-width: 700px;
  margin: 0 auto;
  padding-top: 2rem;
}

.flex {
  display: flex;
  align-items: center;
  padding: 0 0 1rem;
}
.icon {
  width: 30px;
  height: 30px;
  margin-right: 4px;
}

.image-div {
  text-align: right;
}
.image {
  width: 150px;
  height: 150px;
}

.h2 {
  text-align: center;
  padding-top: 1rem;
}

@media only screen and (min-width: 700px){
  .rest {
    display: flex;
    align-items: center;
  }
  .rest .view {
    width: 70%;
  }
}

</style>

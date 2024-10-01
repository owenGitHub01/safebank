<script setup>



</script>

<template>
  <div class="flex">
    <div class="bg">
      <img class="b" src="../images/letter-s.png" alt="">
      <img class="a" src="../images/letter-b.png" alt="">
    </div>
  </div>

</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
}

.flex {
  display: flex;
  align-items: center;
  width: 100%;
  height: 70px;
  background-color: blueviolet;
}
.bg {
  background-color: white;
  width: 70px;
  border-radius: 50%;
}
img {
  width: 40px;
  height: 40px;
}

.a {
  position: absolute;
  left: 25px;
  top: 5px;
}

.b { 
  height: 50px;
}

</style>

<script setup>

import Title from './HomeView/Title.vue';
import Benefits from './HomeView/Benefits.vue';
import Eligible from './HomeView/Eligible.vue';
import Header from './HomeView/Header.vue';

</script>

<template>

  <Header></Header>
  <Title></Title>
  <Benefits></Benefits>
  <Eligible></Eligible>


</template>

<style>

* {
  margin: 0;
  padding: 0;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}
button {
  cursor: pointer;
}

</style>

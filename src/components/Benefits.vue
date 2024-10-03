<script setup>

import support from '../images/Benefits/online.png'
import cashback from '../images/Benefits/credit-card.png'
import isa from '../images/Benefits/atm-card.png'
import protection from '../images/Benefits/verified.png'



const benefits = [
  {
    title: "24/7 Support",
    bio: "No matter where you are, we've got you covered with our 24/7 support.",
    img: support,
    show: true,
    button: false,
    btnMess: ""
  },
  {
    title: "1% Cashback",
    bio: "Enjoy 1% cashback on whatever you spend! ",
    img: cashback,
    show: false,
    button: true,
    btnMess: "Learn How"
  },
  {
    title: "Unbeatable Rates",
    bio: "Our high interest rate Isa's and Lisa's are available now!",
    img: isa,
    show: true,
    button: true,
    btnMess: "Learn More"
  },
  {
    title: "Security",
    bio: "See pride ourselves on our protection and security protecting you from scams!",
    img: protection,
    show: false,
    button: false,
    btnMess: ""
  },
]

</script>

<template>
  <div class="main">
    <div class="border" v-for="item in benefits">
      <div>
        <div class="view-flex" v-if="item.show">

          <div>
            <img :src="item.img" alt="" class="icon">
          </div>
          <div>
            <h1>{{ item.title }}</h1>
            <p class="bio">{{ item.bio }}</p>
            <div class="btn-div" v-if="item.button">
              <button>{{ item.btnMess }}</button>
            </div>
          </div>
        </div>
        <div class="view-flex" v-if="!item.show">
          <div>
            <h1>{{ item.title }}</h1>
            <p class="bio">{{ item.bio }}</p>
            <div class="btn-div" v-if="item.button">
              <button>{{ item.btnMess }}</button>
            </div>
          </div>
          <div>
            <img :src="item.img" alt="" class="icon">
          </div>
        </div>
      </div>
      
    </div>
  </div>

</template>

<style scoped>

* {
  margin: 0;
  padding: 0;
}

.main {
  background-color: rgb(250 250 249);
}

.view-flex {
  display: flex;
  align-items: center;
}  

.icon {
  width: 120px;
  height: 160px;
}

.border {
  width: 80%;
  max-width: 480px;
  margin: 0 auto;
  height: auto;
  padding: 1rem 0 10rem;
  text-align: center;
}
 
.bio {
  width: 90%;
  margin: 0 auto;
}
.btn-div button {
  width: 100px;
  height: 30px;
  border-radius: 12px;
  background-color: aqua;
  border: none;
  margin-top: 1rem;
}


</style>

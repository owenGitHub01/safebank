<script setup>
import { RouterLink } from 'vue-router';

</script>

<template>
  <div class="all">
    <div class="side1">
      <div class="login">
        <h1>Welcome Back!</h1>
        <input type="text" placeholder="Username">
        <p></p>
        <input type="text" placeholder="Password">
        <p class="forgot-p">
          <RouterLink class="forgot" to="/forgotpassword">Forgot password?</RouterLink>
        </p>
        <p class="signup">Still not a user yet?</p>
        <button>
          <RouterLink class="link" to="signup">Sign Up</RouterLink>
        </button>

      </div>
    </div>
    <div class="side2">
      <img src="../images/selfie.png" alt="">
    </div>

  </div>  
</template>

<style scoped>


.all {
  width: 100%;
  height: 100vh;
  background-color: rgb(250 250 249);
}
.link {
  text-decoration: none;
  color: black;
}
.login {
  text-align: center;
  padding-top: 8rem;
}
.login input {
  margin: 16px 0 8px;
  height: 30px;
  width: 260px;
  padding: 0 4px;
  border-radius: 12px;
  border: 1.5px solid black;
}
.forgot-p {
  width: 260px;
  text-align: right;
  margin: 0 auto 2rem;
}
.forgot {
  color: blueviolet;
}

.signup {
  font-size: 20px;
}
button {
  width: 100px;
  margin: 8px 0 0;
  border-radius: 24px;
  height: 24px;
  border: none;
  background-color: rgb(174, 238, 246);
}


.side2 {
  text-align: center;
  
  height: 80vh;
  margin-top: 4rem;
}
.side2 img{
  width: 220px;
  margin: 2rem;
}


@media only screen and (min-width: 800px){

.all {
  display: flex;
  margin: 0 auto;
  
}  
.side1 {
  width: 50%;
}
.login {
  padding-top: 10rem;
}

.side2 {
  margin-top: 0;
  background-color: rgb(214, 217, 217);
  width: 50%;
  padding-top: 15rem;
  
  
}


}

</style>

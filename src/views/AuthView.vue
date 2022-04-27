<template>
   <div :class="$style.overlay"></div>
   <Login v-if="!authCond"/>
   <Register v-if="authCond"/>
</template>

<script setup>
import Login from "../components/authentification/login.vue"
import Register from "../components/authentification/register.vue"
import {ref} from 'vue' 

   let authCond = ref(true);
 



</script>

<style lang="scss" module>
body{
  height:100vh;
  width:100vw;
  background: url("@/assets/loginPic.webp") ;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
.overlay{
  height:100vh;
  width:100vw;
  background-color: hsla(0, 0%, 0%, 0.7);
}
.copyright{
  text-align: center;
  
}
</style>
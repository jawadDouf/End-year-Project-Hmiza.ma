<template>
  <div>
  
  <div :class="login.container">
  <h1>Login</h1>
  <form :class="login.container_form">
       <div :class="login.container_form_email">
       <label :class="login.label">EMAIL:</label>
       <input :class="login.input" type="text" required/>
       </div>
       <div :class="login.container_form_password">
       <label :class="login.label">mot De Passe:</label>
       <input :class="login.input" type="password"  required>
       </div>
        <div :class="login.container_form_checkbox"> 
        <input :class="login.checkbox" type="checkbox" />
        <label :class="login.label">Forgot mot De Passe</label>
        </div>
       <div :class="login.container_form_submit">
        <button :class="login.button">Login</button>
        <div :class="login.registration">
        <p :class="login.register">No Account ?</p>
        <a :class="login.register" @click="$emit('changePage')">Register</a>
        </div>
       </div>       
  </form>
  
  </div>
  </div> 
</template>

<script setup>
import login from "../../modulescss/authentification/login.scss"

const emits = defineEmits(['changePage'])
</script>

<style lang="scss">



</style>
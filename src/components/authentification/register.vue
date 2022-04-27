<template>
   <div :class="register.container">
      <h1 :class="register.container_title">Register</h1>
      <form :class="register.container_form">
       <!-- nom et prenom -->
       
       <div :class="register.field">
       <label :class="register.label">nom:</label>
       <input :class="register.input" type="text"  required>    
       </div>
       <div>
       <label :class="register.label">prenom:</label>
       <input :class="register.input"  type="text"  required>    
       </div>
       <div :class="register.field">
      <!-- email -->
        <label :class="register.label">EMAIL:</label>
        <input :class="register.input"  type="email" required />
      </div>
       <!-- motDePasse -->
       <div :class="register.field">
       <label :class="register.label">mot De Passe:</label>
       <input :class="register.input"  type="password"  required>    
       </div>
       <div :class="register.field">
       <label :class="register.label">Confirm mot De Passe:</label>
       <input :class="register.input" type="password" required>    
       </div>  
       <!-- button -->
       <div :class="register.field">
        <button :class="register.button">Register</button>
        <div :class="register.login">
         <p :class="register.par">Already Registered?</p>
        <a :class="register.a">Login</a>
        </div>
        
       </div>
       
    </form>
   </div>
   
</template>

<script setup>
import register from "../../modulescss/authentification/register.scss"

</script>

<style>

</style>
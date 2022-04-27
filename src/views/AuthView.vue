<template>
  <div>
  <div class="overlay"></div>
  <div class="container">
  <!-- <fa :icon="['fas','circle']" class="container-title"/> -->
  <h1>Login</h1>
  <form class="container-form">
       <div class="container-form-email">
       <label>EMAIL:</label>
       <input type="text" required/>
       </div>
       <div class="container-form-password">
       <label>mot De Passe:</label>
       <input type="password"  required>
       </div>
        <div class="container-form-checkbox"> 
        <input class="checkbox" type="checkbox" />
        <label >Forgot mot De Passe</label>
        </div>
       <div class="container-form-submit">
        <button>Login</button>
        <div class="registration">
        <p class="register">No Account ?</p>
        <a class="register">Register</a>
        </div>
       </div>       
  </form>
  
  </div>
  </div>
  
  
</template>

<script>
export default {
   
}
</script>

<style lang="scss">
@import "@/sass/variables.scss";
@import "@/sass/mexins.scss";
@import "@/sass/mediaquerise.scss";
body{
  height: 100vh;
  width:100vw;
  background: url("@/assets/loginPic.webp") ;
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
.overlay{
  
  height: 100vh;
  width:100vw;
  background-color: hsla(0, 0%, 0%, 0.7);
}
.container{
 
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%,-50%);
    width: 350px;
    height: 450px;
    box-shadow: black 0px 0px 10px;
    @include flex();
    color: white;
    background-color: hsla(0, 0%, 0%, 0);
.container-title{
 width: 50px;
 height: auto;
}
form{
 width: 70%;
}
.container-form-email{
input{    
 padding-block: 6px;
  width: 100%;
  
}
label{
 display: block;
 text-transform: uppercase;
 letter-spacing: 1px;
 font-size: 14px;
}
   margin-block: 30px;
}
.container-form-password{
input{
 padding-block: 6px ;
  width: 100%;
}
label{
 display: block;
 text-transform: uppercase;
 letter-spacing: 1px;
 font-size: 14px;
}
  margin-block: 5px;
}
.container-form-checkbox{
label{
 padding-inline: 5px;
 text-transform: uppercase;
 letter-spacing: 1px;
 font-size: 14px;
}
   
}
.container-form-submit{
 margin-block: 30px;
button{
 display: block;
 @include button($border-radius:0px);
 width: 100%;
 background-color: #4c41c0;
}
.registration{
  margin-block: 20px;
 .register{
 display: inline;
}
a{
  margin-left: 38%;
}
}
}
}
</style>
<template>
  <div class="footer">
  <div class="footer-logo">
  <h2 class="logo">Hmiza.ma</h2>
  <p class="description">Contrary to popular<br> belief, Lorem Ipsum is<br> not simply </p>
  </div>
  <div class="footer-services">
   <div class="service">
  <h2 class="service-title">service</h2>
  <p class="service-par">Examen médical</p>
  <p class="service-par">Clinique d' urgence</p>
  <p class="service-par">Routine check-ups</p>
  <p class="service-par">chirurgies</p>
  </div>
  <div class="service">
  <h2 class="service-title">service</h2>
  <p class="service-par">Examen médical</p>
  <p class="service-par">Clinique d' urgence</p>
  <p class="service-par">Routine check-ups</p>
  <p class="service-par">chirurgies</p>
  </div>
  <div class="service">
  <h2 class="service-title">service</h2>
  <p class="service-par">Examen médical</p>
  <p class="service-par">Clinique d' urgencel</p>
  <p class="service-par">Routine check-ups</p>
  <p class="service-par">chirurgies</p>
  </div>
  <div class="service">
  <h2 class="service-title">service</h2>
  <p class="service-par">Examen médical</p>
  <p class="service-par">Clinique d' urgence</p>
  <p class="service-par">Routine check-ups</p>
  <p class="service-par">chirurgies</p>
  </div>
  </div>
  </div>
  <div class="subFooter">
   <div class="subFooter-firstLine">
    <div class="firstLine-navLinks">
      <ul>
      <li>Acceuil</li>
        <li>Produits</li>
        <li>Profile</li>
        <li>About</li>
      </ul>
        
        </div>
     <div class="firstLine-smLinks">
      <fa :icon="['fab','github']" class="smLink"/>
      <fa :icon="['fab','linkedin']" class="smLink"/>
   </div>   
   </div>
   
   <div class="subFooter-secondLine">
    <p>Copyright © 2022 Hmiza.ma , Tous droits réservés , Made By Jawad.</p>
   </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang=scss>
@import "@/sass/variables.scss";
@import "@/sass/mexins.scss";
@import "@/sass/mediaquerise.scss";
.footer{
  background-color: #2D4487;
  color: white;
  margin-top: 20px;
  margin-bottom: 5px;
  padding-top: 20px;
  padding-bottom: 90px;
  @include flex($direction:row);
  gap: 15%;
 @include tablet{
   gap: 3%;
   flex-wrap: wrap;
 }
 @include smallTablet{
  gap: 3%;
 }
 @include mobile{
  gap: 5%;
 }
}
.footer-logo{
 align-self: flex-start;
 margin-top: 10px;
 @include tablet{
  align-self: flex-start;
 
 }
.logo{
 margin-block: 10px;
 @include mobile{
   font-size: 20px;
 }
}
.description{
 margin-block:10px;
 @include mobile{
   font-size: 14px;
 }
}
}
.footer-services{
 display: grid;
 grid-template-columns: repeat(4,1fr);
 @include mobile{
  grid-template-columns:repeat(2,1fr);
 }
 @include smallTablet{
   grid-template-columns: repeat(2,1fr);
 }
.service{
 margin-inline: 35px;
 @include tablet {
   margin-inline: 20px;
 }
 @include smallTablet{
   margin-inline:15px;
 }
 @include mobile{
  margin-inline: 8px;
 }
.service-title{
  margin-block: 20px;
  @include mobile{
   font-size: 20px;
  }
}
.service-par{
 margin-block: 10px;
 @include mobile{
  font-size:12px;
 }
}
}

}
.subFooter{
 background-color: #2D4487;
 color: white;
 display: grid;
 grid-template-rows: 2fr 1fr;
.subFooter-firstLine{
  @include flex($direction:row,$justify-content:space-between);
.firstLine-navLinks{
ul{
li{
 display: inline;
 list-style: none;
 margin-inline: 15px;
 @include mobile{
  font-size: 14px;
  margin-inline: 10px;
 }
}
}
}
.firstLine-smLinks {
.smLink{
  width: 25px;
  height: auto;
  margin-inline: 15px;
  cursor: pointer;
@include mobile{
  width: 18px;
  height: auto;
  margin-inline: 10px;
 }
&:hover{
 color: rgb(159, 158, 158);
}
}
 

}
}
.subFooter-secondLine{
p{
 text-align: center;
 @include mobile{
  font-size:12px;
 }
}
}
}
</style>
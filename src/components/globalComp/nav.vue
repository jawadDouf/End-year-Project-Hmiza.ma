<template>
  
  <div id="nav">
  <ul>
    <li>Logo</li>
    <li>Acceuil</li>
    <li>Produits</li>
    <li>Profile</li>
    <li>A propos</li>
    <li><button>   
    Register
    </button></li>
  </ul> 
  <div class="cover">
    <div class="cover-leftSide">
     <h1>Samsung Galaxy Note 10+ with<br>256 GB (U.S. Warranty), Aura<br> Black/ Note10+ (Renewed)</h1>
     <p>Contrary to popular belief, Lorem Ipsum is not<br> simply random text. It has roots in a piece of<br>classical Latin literature from 45 BC, making it<br>  has roots in a piece of classical Latin literature<br> from 45 BC, making it </p>
     <button>Check the product</button>
    </div>
    <div class="cover-rightSide">
    
    <img src="@/assets/coverFirstImage.png" alt="phone image" />
    <div class="nav-prices">
  <div class="onePrice">
  <fa :icon="['fab','amazon']" class="amazon"/>
  <p>:300$</p>
  </div>
  <div class="onePrice">
  <fa :icon="['fab','shopify']" class="amazon"/>
  <p>:300$</p>
  </div>
  <div class="onePrice">
  <fa :icon="['fab','ebay']" class="amazon"/>
  <p>:300$</p>
  </div>
  <div class="onePrice">
  <fa :icon="['fab','apple']" class="amazon"/>
  <p>:300$</p>
  </div>
  <div class="onePrice">
  <fa  :icon="['fab','amazon']" class="amazon"/>
  <p>:300$</p>
  </div>
  </div>
    </div>
 
  </div>
   <br>
  </div>
 

</template>

<script setup>


</script>
<style lang="scss" scoped>
@import "@/sass/variables.scss";
@import "@/sass/mexins.scss";
@import "@/sass/mediaquerise.scss";
.router{
 text-decoration: none;
 color:$primary-color;
}
#nav{
font-family: $primary-font;
background-color: #2D4487;
height:auto;
width: 95%;
margin: auto;
border-radius: 10px;
margin-top:10px;
ul{
 font-weight: 500;
 padding-top:20px;
 list-style: none;
 @include flex($direction:row);
 gap: 10%;
 color: white;
button{
 @include button($horizontal-padding:20px);
 background-color: white;
 color: $primary-color;
}
}
.cover{
@include flex($direction:row);
gap: 5%;
.cover-leftSide{
@include flex($aligin-items:flex-start);
margin-bottom: 20px;
gap: 20px;
h1{
 color:white;
}
p{
 color: white;
 font-size: 12px;
 line-height: 1.75;
}
button{
@include button($horizontal-padding:50px,$vertical-padding:12px,$border-radius:0px);
 background-color: white;
 color: $primary-color;
}
}
.cover-rightSide{
margin-top:40px;
@include flex($direction:row);
img{
 width:70%;
 height:auto;
}
}
}
}
.nav-prices{
@include flex();
gap: 30px;
align-self: flex-start;
.onePrice{
@include flex($direction:row);
gap: 8px;
p{
align-self:flex-end;
color: white;
font-size: 1.2em;
font-weight:550;
}
}

.amazon{
color: white;
width: 50px;
height: auto;
}
}
.p{
 color: white;
 text-align: center;
}


</style>
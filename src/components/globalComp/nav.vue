<template>

  <div id="nav">
  <ul>
    <li>Logo</li>
    <li>Acceuil</li>
    <li>Produits</li>
    <li>Profile</li>
    <li>A propos</li>
    <li><button>Register</button></li>
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
 
 <div class="secSection">
 <h1 class="secSection-title">Our Services</h1>
 <div class="secSection-elements">
 <div class="secSection-leftside">
 <h1 class="secSection-leftside-bigTitle">We are trying to make your<br> custumer Experiance in the<br> internet easier</h1>
 <p class="secSection-leftside-par">Contrary to popular belief, Lorem Ipsum is not<br> simply random text. It has roots in a piece of<br> classical Latin </p>
 <div class="secSection-leftside-checkpoints">
  <p class="par"><fa :icon="['fas','circle-check']" class="check"/><span>same shit i didn’t think about it yet</span></p>
 <p class="par"><fa :icon="['fas','circle-check']" class="check"/><span>some shit i didn’t think about it yet</span></p>
 <p class="par"><fa :icon="['fas','circle-check']" class="check"/><span>some shit i didn’t think about it yet</span></p>
 </div>
 <div class="secSection-leftside-button">
 <button>Learn More about us</button>
 </div>
 
 </div>
 <div class="secSection-rightside">
   <div class="secSection-rightside-service">
     <img src="@/assets/received1.png" alt="service pic" style="width:110px;height:auto;"/>
     <h3>Search for a product</h3>
     <p>Contrary to popular<br> belief, Lorem Ipsum is<br> not</p>
     <a href="">Start from here</a>
   </div>
   <div class="secSection-rightside-service">
     <img src="@/assets/services1.png" alt="service pic" style="width:125px;height:auto;"/>
     <h3>Search for a Service</h3>
     <p>Contrary to popular<br> belief, Lorem Ipsum is<br> not</p>
     <a href="">Start from here</a>
   </div>
   <div class="secSection-rightside-service">
     <img src="@/assets/like1.png" alt="service pic" style="width:100px;height:auto;"/>
     <h3>Review a product </h3>
     <p>Contrary to popular<br> belief, Lorem Ipsum is<br> not</p>
     <a href="">Start from here</a>
   </div>
   <div class="secSection-rightside-service">
     <img src="@/assets/price-tags1.png" alt="service pic" style="width:90px;height:auto;"/>
     <h3>Compare Products</h3>
     <p>Contrary to popular<br> belief, Lorem Ipsum is<br> not</p>
     <a href="">Start from here</a>
   </div>
 </div>
 </div>
 </div>
  <div class="thirdsection">
  <h1 class="thirdsection-bigTitle">We Can Help you to Improve Your business , BY<br> Creating a business Account</h1>
  <p class="thirdsection-par">Contrary to popular belief, Lorem Ipsum is not simply </p>
  <div class="thirdsection-checkpoints">
  <p class="par"><fa :icon="['fas','circle-check']" class="check"/><span>Create A Business Account</span></p>
 <p class="par"><fa :icon="['fas','circle-check']" class="check"/><span>Fill And Organize Your Stock</span></p>
 <p class="par"><fa :icon="['fas','circle-check']" class="check"/><span>Add Posts and blogs About your Buisinesse</span></p>
 </div>
  <button class="thirdsection-button">Start from here</button>
  </div>  
  <div class="fourthsection">
    <h1 class="fourthsection-bigTitle">The Websites Prices Available in our Website</h1>
    <div class="fourthsection-logos">
    <fa :icon="['fab','ebay']" class="logo"/>
    <fa :icon="['fab','Amazon']" class="logo"/>
    <fa :icon="['fab','apple']" class="logo"/>
    <fa :icon="['fab','shopify']" class="logo"/>
    <fa :icon="['fab','ebay']" class="logo"/>
    <fa :icon="['fab','amazon']" class="logo"/>
    <fa :icon="['fab','shopify']" class="logo"/>
    <fa :icon="['fab','amazon']" class="logo"/>
    <fa :icon="['fab','ebay']" class="logo"/>
    </div>
    <button class="fourthsection-button">Learn More >></button>
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
.secSection{
.secSection-title{
  padding-top:30px;
  text-align: center;
  font-size: 2rem;
 @include mobile{
   font-size: 30px;
 }
  }
.secSection-elements{
  padding-top: 20px ;
  gap: 15%;
 @include flex($direction:row);
@include tablet{
 @include flex($direction:column);
}
@include mobile{
 @include flex($direction:column);
}
 
.secSection-leftside{
  display: grid;
  grid-template-rows: repeat(4, 1fr);
@include mobile{
 height:260px;
}
.secSection-leftside-bigTitle{
 font-size:30px;
 @include tablet{
 text-align:center;
}
@include mobile{
 text-align:center;
 font-size:25px;
}

}
.secSection-leftside-par{
 margin-block:15px;
 font-size: 18px;
 @include tablet{
 text-align:center;
}
 @include mobile{
  display: none;
 }
}
.secSection-leftside-checkpoints{

.par{
margin-block:10px;
@include tablet{
 text-align:center;
}
@include mobile{
 text-align:center;
}
span{
padding-left:8px ;
}
.check{
 color: #554BBF;
 

}
}
}
.secSection-leftside-button{
 margin-block: 15px;
 @include tablet{
 text-align:center;
}
@include mobile{
 text-align:center;
}
button{
 @include button($vertical-padding:12px,$horizontal-padding:20px,$border-radius:5px);
 background-color: #554BBF;
 
}

}

}
.secSection-rightside{
 display: grid;
 grid-template-columns: repeat(2, 1fr);
@include tablet{
 grid-template-columns: repeat(4, 1fr);
 @include flex($direction:row);
 flex-wrap: wrap;
}
@include mobile{
 display: grid;
 grid-template-columns: repeat(1, 1fr);
 width: 70%;
}
.secSection-rightside-service{
   border: solid 1px grey;
   border-radius:5px;
   padding: 20px;
   margin:20px ; 
@include mobile{
   @include flex;
   text-align: center;
}

a{
color: #554BBF;
font-size:20px;
font-weight:400;
}
}
}
}
}
.thirdsection{
 margin-block: 20px;
 padding-block:30px ;
 background-color: #2D4487;
 @include flex;
 color: white;
.thirdsection-bigTitle{
 text-align: center;
}
.thirdsection-par{
 margin-block:10px ;
}
.thirdsection-checkpoints{
 margin-block: 5px;
 
.par{
margin-block:10px ;
}
span{
padding-left:8px ;
}
.check{
 color: #49FF00;
 

}

}
.thirdsection-button{
  margin-block: 10px;
  @include button($vertical-padding:10px,$horizontal-padding:40px,$border-radius:5px);
  background-color:white;
  color: $primary-color;
  
}
}
.fourthsection{
 
.fourthsection-bigTitle{
 text-align: center;
 margin-block: 35px;
}
.fourthsection-logos{
 margin-inline: 10%;
 @include flex($direction:row);
 gap: 15%;
 flex-wrap: wrap;
 
.logo{
 width: 80px;
 height: auto;
}
}
.fourthsection-button{
 @include button($vertical-padding:12px,$horizontal-padding:40px,$border-radius:5px);
 margin-block:45px;
 margin-left: 43%;
 background-color: #2D4487;
 @include mobile{
  margin-left:30%;
 
 }
}
}

</style>
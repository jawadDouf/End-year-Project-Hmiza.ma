<template>
  <nav>
    
  </nav>
  <router-view/>
</template>
<script>
import Nav from '@/components/globalComp/nav.vue';
import Footer from './components/globalComp/footer.vue';

export default {
components : {
  Nav,
Footer
}
}
</script>

<style lang="scss">
@import "@/sass/variables.scss";
@import "@/sass/mexins.scss";
@import "@/sass/mediaquerise.scss";
*{
  margin: 0;
  padding: 0;
  
}



</style>

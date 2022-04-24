<template>
  <nav>
    <Nav />
  </nav>
  <router-view/>
</template>
<script>
import Nav from '@/components/globalComp/nav.vue';

export default {
components : {
  Nav
}
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}



</style>

<template>
  <NavBar/>
  <router-view/>
</template>
<script>
import NavBar from '@/components/NavBar-comp.vue'
export default {
  components: {NavBar}
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}


</style>

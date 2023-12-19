<template>
  <div class="side-ribbon-tab">
    Ribbon section
  </div>
  <MyFooter></MyFooter>
</template>

<script>
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyFooter
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>

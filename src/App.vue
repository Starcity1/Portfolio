<template>
  <main>
    <SideRibbon v-if="showRibbon"></SideRibbon>
    <HomeView></HomeView>
    <MyFooter></MyFooter>
  </main>
</template>

<script>
import HomeView from './components/Home.vue';
import MyFooter from './components/MyFooter.vue';
import SideRibbon from './components/SideRibbon.vue';

export default {
  name: 'App',
  components: {
    MyFooter,
    SideRibbon,
    HomeView,
  },
  data() {
    return {
      showRibbon: true,
      showHome: true,
      showAboutMe: false,
      showResearch: false,
      showProjects: false,
      showSingapore: false,
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* Prevent Border box from increasing size */
  -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
  -moz-box-sizing: border-box;    /* Firefox, other Gecko */
  box-sizing: border-box;         /* Opera/IE 8+ */
}

main {
  overflow: hidden;
  width: 100vw;
  height: 100vh;
}
</style>

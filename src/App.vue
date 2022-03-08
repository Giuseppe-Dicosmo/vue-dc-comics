<template>
  <div id="app">
    <HeaderNav />
    <MainContent />
    <MainShop />
    <MainInfo />
    <footerSocial />
  </div>
</template>

<script>
import HeaderNav from "./components/HeaderNav.vue";
import MainContent from "./components/MainContent.vue";
import MainShop from "./components/MainShop.vue";
import MainInfo from "./components/MainInfo.vue";
import footerSocial from "./components/footerSocial.vue";

export default {
  name: "App",
  components: {
    HeaderNav,
    MainContent,
    MainShop,
    MainInfo,
    footerSocial,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  max-width: 80%;
  margin: 0 auto;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>

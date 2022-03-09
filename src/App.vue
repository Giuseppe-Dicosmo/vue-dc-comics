<template>
  <div id="app">
    <HeaderNav />
    <MainContent />
    <MainShop />
    <footerInfo />
    <footerSocial />
  </div>
</template>

<script>
import HeaderNav from "./components/HeaderNav.vue";
import MainContent from "./components/MainContent.vue";
import MainShop from "./components/MainShop.vue";
import footerInfo from "./components/footerInfo.vue";
import footerSocial from "./components/footerSocial.vue";

export default {
  name: "App",
  components: {
    HeaderNav,
    MainContent,
    MainShop,
    footerInfo,
    footerSocial,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/mix.scss";

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container{
  @include container;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>

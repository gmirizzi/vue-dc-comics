<template>
  <div id="app">
    <AppHeader />
    <MainContent />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import MainContent from "./components/MainContent.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    MainContent,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./assets/css/_reset.css";
#app {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}
.container {
  width: 1000px;
  margin: 0 auto;
  display: flex;
}
</style>

<template>
  <div id="app">
    <AppHeader />
    <MainContent />
    <BlueBar />
    <AppFooter />
    <BottomBar />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import MainContent from "./components/MainContent.vue";
import AppFooter from "./components/AppFooter.vue";
import BottomBar from "./components/BottomBar.vue";
import BlueBar from "./components/BlueBar.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    MainContent,
    AppFooter,
    BottomBar,
    BlueBar,
  },
};
</script>

<style lang="scss">
@import "./assets/css/_reset.css";
#app {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
}
.container {
  width: 1100px;
  margin: 0 auto;
  display: flex;
}
</style>

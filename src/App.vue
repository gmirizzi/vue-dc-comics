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

<style lang="scss"></style>

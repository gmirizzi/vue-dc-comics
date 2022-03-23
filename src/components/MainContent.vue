<template>
  <main>
    <div id="jumbotron"></div>
    <div class="container">
      <CardSerie />
    </div>
  </main>
</template>

<script>
import CardSerie from "./CardSerie.vue";

export default {
  name: "MainContent",
  components: {
    CardSerie,
  },
};
</script>

<style scoped lang="scss">
main {
  background-color: black;
  color: white;
  #jumbotron {
    height: 400px;
    background-image: url("./../assets/img/jumbotron.jpg");
    background-position-x: center;
  }
}
</style>

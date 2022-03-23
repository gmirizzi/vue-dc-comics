<template>
  <div class="card">
    <img :src="img" alt="" />
    <div class="serie">{{ serie }}</div>
  </div>
</template>

<script>
export default {
  name: "CardSerie",
  props: {
    img: String,
    serie: String,
  },
};
</script>

<style scoped lang="scss">
.card {
  width: 150px;
  margin-bottom: 2.5em;
  img {
    width: 100%;
    height: 150px;
  }
  .serie {
    text-transform: uppercase;
    margin-top: 1em;
    font-size: 0.7rem;
  }
}
</style>

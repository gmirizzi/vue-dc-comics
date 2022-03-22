<template>
  <div id="bottombar">
    <div class="container">
      <a href="#">SIGN-UP NOW!</a>
      <div id="social">
        <h1>FOLLOW US</h1>
        <a href="#"
          ><img src="./../assets/img/footer-facebook.png" alt="logo facebook"
        /></a>
        <a href="#"
          ><img src="./../assets/img/footer-twitter.png" alt="logo twitter"
        /></a>
        <a href="#"
          ><img src="./../assets/img/footer-youtube.png" alt="logo youtube"
        /></a>
        <a href="#"
          ><img src="./../assets/img/footer-pinterest.png" alt="logo pinterest"
        /></a>
        <a href="#"
          ><img src="./../assets/img/footer-periscope.png" alt="logo periscope"
        /></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomBar",
};
</script>

<style scoped lang="scss">
#bottombar {
  background-color: #303030ff;
  padding: 1em;
}
.container {
  justify-content: space-between;
  align-items: center;
  #social {
    display: flex;
    align-items: center;
    gap: 1em;
    h1 {
      color: #0282f9ff;
      font-size: 1rem;
    }
  }
}
.container > a {
  text-decoration: none;
  color: white;
  border: 1px solid #0282f9ff;
  padding: 0.5em;
}
</style>

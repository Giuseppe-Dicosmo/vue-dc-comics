<template>
  <main class="container-Content">
    <div class="container">
      <a href="#">SING-UP NOW!</a>
      <div class="container-social">
        <span>FOLLOW US</span>
        <figure>
          <img src="../assets/footer-facebook.png" alt="" />
          <img src="../assets/footer-twitter.png" alt="" />
          <img src="../assets/footer-youtube.png" alt="" />
          <img src="../assets/footer-pinterest.png" alt="" />
          <img src="../assets/footer-periscope.png" alt="" />
        </figure>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainContent",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-Content {
  height: 10vh;
  width: 100%;
  background-color: #303030;
  color: white;
  display: flex;
  align-items: center;

  .container {
    display: flex;
    justify-content: space-between;
    flex-grow: 1;
    // border: 1px solid red;
  }

  a {
    padding: 10px;
    color: white;
    font-size: 15px;
    border: 3px solid #0282f9;
    text-decoration: none;
  }
  .container-social {
    display: flex;
    align-items: center;
    gap: 20px;
    height: 50%;

    figure {
      display: flex;
      gap: 10px;
    }
  }
}
</style>

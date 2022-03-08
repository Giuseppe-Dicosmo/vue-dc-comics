<template>
  <main class="container-Content">
    <div class="container">
      <div class="info">
        <div class="lista1">
          <ul>
            <h3>cd comics</h3>
            <li><a href="">Characters</a></li>
            <li><a href="">Comics</a></li>
            <li><a href="">Movies</a></li>
            <li><a href="">TV</a></li>
            <li><a href="">Games</a></li>
            <li><a href="">Videos</a></li>
            <li><a href="">News</a></li>
          </ul>
          <ul>
            <h3>shop</h3>
            <li><a href="">Shop DC</a></li>
            <li><a href="">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="lista2">
          <ul>
            <h3>cd</h3>
            <li><a href="">Terms Of Use</a></li>
            <li><a href="">Privacy policy (New) </a></li>
            <li><a href="">ad Choices</a></li>
            <li><a href="">advertising</a></li>
            <li><a href="">Jobs</a></li>
            <li><a href="">Subscriptions</a></li>
            <li><a href="">Talent Workshops</a></li>
            <li><a href="">CPSC Certificates</a></li>
            <li><a href="">Ratings</a></li>
            <li><a href="">shop Help</a></li>
            <li><a href="">Contact Us</a></li>
          </ul>
        </div>
        <div class="lista3">
          <ul>
            <h3>sistes</h3>
            <li><a href="">DC</a></li>
            <li><a href="">MAD Magazine</a></li>
            <li><a href="">DC Kids</a></li>
            <li><a href="">DC Universe</a></li>
            <li><a href="">DC Power visa</a></li>
          </ul>
        </div>
      </div>

      <div class="logo-bg"></div>
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
  height: 55vh;
  width: 100%;
  background: url("../assets/footer-bg.jpg") no-repeat center;
  background-size: cover;
  color: white;
  display: flex;
  align-items: center;

  .container {
    display: flex;
    width: 100%;
    height: 100%;

    .info {
      width: 35%;
      display: flex;
      // border: 1px solid red;
      gap: 20px;

      ul {
        list-style-type: none;

        h3 {
          text-transform: uppercase;
          margin: 10px 0;
        }

        a {
          font-size: 13px;
          color: #8f8e8e;
          text-decoration: none;
        }
      }
    }

    .logo-bg {
      flex-grow: 1;
      background: url("../assets/dc-logo-bg.png") no-repeat right center;
      background-size: 60%;
      // border: 1px solid yellow;
    }
  }
}
</style>

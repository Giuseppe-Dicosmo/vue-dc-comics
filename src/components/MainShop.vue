<template>
  <main class="container-Content">
    <div class="container">
      <ul class="container-Shop">
        <li>
          <a href="#">
            <figure class="img-Shop">
              <img src="../assets/buy-comics-digital-comics.png" alt="" />
            </figure>
            <span> lorem </span>
          </a>
        </li>
        <li>
          <a href="#">
            <figure class="img-Shop">
              <img src="../assets/buy-comics-merchandise.png" alt="" />
            </figure>
            <span> lorem </span>
          </a>
        </li>
        <li>
          <a href="#">
            <figure class="img-Shop">
              <img src="../assets/buy-comics-subscriptions.png" alt="" />
            </figure>
            <span> lorem </span>
          </a>
        </li>
        <li>
          <a href="#">
            <figure class="img-Shop">
              <img src="../assets/buy-comics-shop-locator.png" alt="" />
            </figure>
            <span> lorem </span>
          </a>
        </li>
        <li>
          <a href="#">
            <figure class="img-Shop">
              <img src="../assets/buy-dc-power-visa.svg" alt="" />
            </figure>
            <span> lorem </span>
          </a>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainShop",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-Content {
  height: 15vh;
  width: 100%;
  background-color: #0282f9;
  color: white;
  display: flex;
  align-items: center;

  .container {
    flex-grow: 1;
    height: 100%;
  }

  .container-Shop {
    display: flex;
    justify-content: space-around;
    height: 100%;

    li {
      display: flex;

      a {
        display: flex;
        align-items: center;
        flex-direction: row;
        gap: 10px;
        text-decoration: none;
        color: white;

        figure {
          height: 50%;

          img {
            height: 100%;
          }
        }
      }
    }
  }
}
</style>

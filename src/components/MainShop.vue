<template>
  <main class="container-Content">
    <div class="container">
      <ul class="container-Shop">
        <li v-for="(link, i) in links" :key="i">
          <a href="#">
            <figure class="img-Shop">
              <img :src="require('../assets/' + link.img)" alt="" />
            </figure>
            {{ link.text }}
          </a>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainShop",
  data() {
    return {
      links: [
        {
          img: "buy-comics-digital-comics.png",
          text: "digital comics",
          href: "#",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "dc merchandise",
          href: "#",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "subscription",
          href: "#",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "comic shop locator",
          href: "#",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "dc power visa",
          href: "#",
        },
      ],
    };
  },
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
        flex-flow: row wrap;
        font-size: 13px;
        gap: 10px;
        text-decoration: none;
        color: white;
        text-transform: uppercase;
        padding: 0 10px;

        &:hover {
          background: rgba($color: #ffffff15, $alpha: 0.5);
        }

        figure {
          height: 35%;

          img {
            height: 100%;
          }
        }
      }
    }
  }
}
</style>

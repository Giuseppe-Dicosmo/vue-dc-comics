<template>
  <main class="container-Content">
    <div class="container">
      <a class="button" href="#">{{button}}</a>
      <div class="container-social">
        <span>FOLLOW US</span>
        <figure v-for="(link, i) in links" :key="i">
          <a :href="link.href"
            ><img :src="require('../assets/' + link.img)" alt=""
          /></a>
        </figure>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainContent",
  data() {
    return {
      button: "SING-UP NOW!",
      links: [
        {
          img: "footer-facebook.png",
          href: "#",
        },
        {
          img: "footer-twitter.png",
          href: "#",
        },
        {
          img: "footer-youtube.png",
          href: "#",
        },
        {
          img: "footer-pinterest.png",
          href: "#",
        },
        {
          img: "footer-periscope.png",
          href: "#",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
$brand_color: white;
$brand_blue: #0282f9;

.container-Content {
  height: 10vh;
  width: 100%;
  background-color: #303030;
  color: $brand_color;
  display: flex;
  align-items: center;

  .container {
    display: flex;
    justify-content: space-between;
    flex-grow: 1;

    .button {
      padding: 10px;
      color: $brand_color;
      font-size: 15px;
      border: 3px solid $brand_blue;
      text-decoration: none;
    }
    .container-social {
      display: flex;
      align-items: center;
      gap: 20px;
      height: 50%;

      span {
        color: $brand_blue;
      }

      figure {
        display: flex;
        gap: 10px;
      }
    }
  }
}
</style>

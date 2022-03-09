<template>
  <footer class="container-Content">
    <div class="container">
      <div class="container-info">
        <div class="info">
          <div class="lista1">
            <ul>
              <h3>{{ titolo1 }}</h3>
              <li v-for="(link, i) in lista1" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
            <ul>
              <h3>{{ titolo2 }}</h3>
              <li v-for="(link, i) in lista1_2" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="lista2">
            <ul>
              <h3>{{ titolo3 }}</h3>
              <li v-for="(link, i) in lista2" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="lista3">
            <ul>
              <h3>{{ titolo4 }}</h3>
              <li v-for="(link, i) in lista3" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>

      <div class="logo-bg"></div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "MainContent",
  data() {
    return {
      titolo1: "cd comics",
      titolo2: "shop",
      titolo3: "cd",
      titolo4: "sistes",
      lista1: [
        {
          text: "Characters",
          href: "#",
        },
        {
          text: "Comics",
          href: "#",
        },
        {
          text: "Movies",
          href: "#",
        },
        {
          text: "TV",
          href: "#",
        },
        {
          text: "Games",
          href: "#",
        },
        {
          text: "videos",
          href: "#",
        },
        {
          text: "News",
          href: "#",
        },
      ],
      lista1_2: [
        {
          text: "Shop DC",
          href: "#",
        },
        {
          text: "Shop DC Collectibles",
          href: "#",
        },
      ],
      lista2: [
        {
          text: "Terms Of Use",
          href: "#",
        },
        {
          text: "Privacy policy (New)",
          href: "#",
        },
        {
          text: "ad Choices",
          href: "#",
        },
        {
          text: "advertising",
          href: "#",
        },
        {
          text: "Jobs",
          href: "#",
        },
        {
          text: "Subscriptions",
          href: "#",
        },
        {
          text: "Talent Workshops",
          href: "#",
        },
        {
          text: "CPSC Certificates",
          href: "#",
        },
        {
          text: "Ratings",
          href: "#",
        },
        {
          text: "shop Help",
          href: "#",
        },
        {
          text: "Contact Us",
          href: "#",
        },
      ],
      lista3: [
        {
          text: "DC",
          href: "#",
        },
        {
          text: "MAD Magazine",
          href: "#",
        },
        {
          text: "DC Kids",
          href: "#",
        },
        {
          text: "DC Universe",
          href: "#",
        },
        {
          text: "DC Power visa",
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

    .container-info {
      width: 35%;
      display: flex;
      align-items: center;
    }

    .info {
      width: 100%;
      display: flex;
      justify-content: space-between;
      gap: 15px;

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

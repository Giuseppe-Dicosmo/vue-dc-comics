<template>
  <header>
    <div class="container-header">
      <nav class="container">
        <figure>
          <img src="../assets/dc-logo.png" alt="" />
        </figure>
        <ul>
          <li v-for="(link, i) in links" :key="i">
            <a :href="link.href"> {{ link.text }} </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderNav",
  data() {
    return {
      links: [
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
          text: "collectibles",
          href: "#",
        },
        {
          text: "videos",
          href: "#",
        },
        {
          text: "fans",
          href: "#",
        },
        {
          text: "news",
          href: "#",
        },
        {
          text: "shop",
          href: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container-header {
  height: 10vh;
  width: 100%;

  .container {
    display: flex;
    flex-flow: row wrap;
    align-self: center;
    height: 100%;
    list-style-type: none;
  }

  figure {
    flex-grow: 1;
    height: 100%;
    padding: 10px 0;

    img {
      height: 100%;
    }
  }

  ul {
    display: flex;
    flex-flow: row wrap;
    gap: 10px;
  }

  li {
    display: flex;
    align-items: center;
    border-bottom: 5px solid transparent;

    &:hover,
    &:nth-child(2) {
      border-bottom: 5px solid #0282f9;
    }

    a {
      font-size: 13px;
      text-transform: uppercase;
      text-decoration: none;

      &:hover {
        color: #0282f9;
      }
    }
  }
}
</style>

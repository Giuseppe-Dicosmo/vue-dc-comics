<template>
  <li>
    <figure>
      <img :src="src" alt="" />
    </figure>
    <h5>{{ title }}</h5>
  </li>
</template>

<script>
export default {
  props: ["title", "src"],
  created() {
    console.log(this.title, this.src);
  },
};
</script>

<style scoped lang="scss">
li {
  width: calc((100% / 6) - 17px);
  cursor: pointer;
  // border: 1px solid fuchsia;
}

figure {
  aspect-ratio: 1 / 1;
  overflow: hidden;
  // border: 1px solid green;

  img {
    max-width: 100%;
  }
}

h5 {
  margin-top: 15px;
  text-transform: uppercase;
}
</style>

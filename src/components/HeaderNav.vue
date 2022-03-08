<template>
  <header>
    <div class="container-header">
      <nav class="container">
        <figure>
          <img src="../assets/dc-logo.png" alt="" />
        </figure>
        <ul>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
          <li><a href="#">lorem</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderNav",
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

      &:hover,
      &:nth-child(2) {
        border-bottom: 5px solid #0282f9;
      }

      a {
        text-decoration: none;

        &:hover {
          color: #0282f9;
        }
      }
    }
  }


</style>

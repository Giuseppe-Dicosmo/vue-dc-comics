<template>
  <section class="container-Content">
    <span class="Content-jumbotron"></span>
    <div class="container">
      <button class="button-series">Content series</button>
      <ul>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
        <li>
          <figure>
            <img
              src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX"
              alt=""
            />
          </figure>
          <p>lorem lorem</p>
        </li>
      </ul>
    </div>
    <button class="button-more">load more</button>
  </section>
</template>

<script>
export default {
  name: "MainContent",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-Content {
  height: 150vh;
  width: 100%;
  background-color: black;
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;

  .Content-jumbotron {
    background: url("../assets/jumbotron.jpg") no-repeat top center;
    background-size: cover;
    width: 100%;
    height: 40%;
  }

  .container {
    width: 100%;
    height: 45%;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    // border: 1px solid red;

    .button-series {
      border: 1px solid #0282f9;
      background: #0282f9;
      color: white;
      text-transform: uppercase;
      font-size: 20px;
      padding: 10px;
      cursor: pointer;
      position: absolute;
      bottom: 95%;
      left: 0;
      transform: translate(0, -70%);
    }

    ul {
      width: 95%;
      height: 100%;
      display: flex;
      flex-flow: row wrap;
      gap: 20px;
      list-style-type: none;
      // border: 1px solid yellow;

      li {
        width: calc((100% / 6) - 17px);
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
    }
  }

  .button-more {
    border: 1px solid #0282f9;
    background: #0282f9;
    color: white;
    text-transform: uppercase;
    font-size: 13px;
    padding: 10px 35px;
    cursor: pointer;
  }
}
</style>

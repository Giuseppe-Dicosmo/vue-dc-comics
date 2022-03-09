<template>
  <section class="container-Content">
    <span class="Content-jumbotron"></span>
    <div class="container">
      <button>Content series</button>
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
  align-items: center;

  .Content-jumbotron {
    background: url("../assets/jumbotron.jpg") no-repeat top center;
    background-size: cover;
    width: 100%;
    height: 40%;
  }

  .container {
    width: 100%;
    height: 100%;
    border: 1px solid red;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;

    button {
      border: 1px solid #0282f9;
      background: #0282f9;
      color: white;
      text-transform: uppercase;
      font-size: 20px;
      padding: 10px;
      position: absolute;
      bottom: 94%;
      left: 0;
      transform: translate(0, -50%);
    }

    ul {
      width: 95%;
      display: flex;
      flex-flow: row wrap;
      gap: 20px;
      border: 1px solid yellow;
      list-style-type: none;

      li {
        width: calc((100% / 6) - 20px);
        height: calc((100% / 2) - 20px);
        border: 1px solid fuchsia;
      }

      figure {
        // height: 50%;
        border: 1px solid green;
        overflow: hidden;

        img {
          max-width: 100%;
        }
      }
    }
  }
}
</style>

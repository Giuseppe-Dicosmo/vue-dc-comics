<template>
  <main class="container-Content">
    <div class="container">
      <div class="">
        --> Content goes here
      </div>
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
  height: 10vh;
  width: 100%;
  background-color: black;
  color: white;
  display: flex;
  align-items: center;

  .container {
    flex-grow: 1;
  }

}
</style>

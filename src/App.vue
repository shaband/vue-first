<template>
  <div id="app">
    <header-app/>
    <content-app/>
    <footer-app/>
  </div>
</template>

<script>
import Header from "./components/layouts/header.vue";
import content from "./components/layouts/content.vue";
import footer from "./components/layouts/footer.vue";

export default {
  name: "app",
  components: {
    "header-app": Header,
    "content-app": content,
    "footer-app": footer
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
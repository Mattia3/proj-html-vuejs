<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "style/variables";
@import "~font-awesome/css/font-awesome.min.css";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>

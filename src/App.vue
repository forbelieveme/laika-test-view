<template>
  <Header title="HW"></Header>
  <Carousel></Carousel>
  <Categories></Categories>
  <Footer></Footer>
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Carousel from "./components/Carousel.vue";
import Categories from "./components/Categories.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
    Carousel,
    Categories,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

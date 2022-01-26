<template>
  <Header></Header>
  <Carousel></Carousel>
  <Categories :categories="categories"></Categories>
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
  data() {
    return {
      categories: [],
    };
  },
  created() {
    this.categories = [
      {
        id: 1,
        title: "Alimento",
        url: "#",
      },
      {
        id: 2,
        title: "Snacks",
        url: "#",
      },
      {
        id: 3,
        title: "Farmapet",
        url: "#",
      },
      {
        id: 4,
        title: "Cuidado e Higiene",
        url: "#",
      },
      {
        id: 5,
        title: "Juguetes",
        url: "#",
      },
      {
        id: 6,
        title: "Accesorios",
        url: "#",
      },
      {
        id: 7,
        title: "Para PetLovers",
        url: "#",
      },
    ];
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
}

.bg_purple {
  background-color: #603e85 !important;
}
</style>

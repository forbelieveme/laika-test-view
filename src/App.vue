<template>
  <Header title="HW"></Header>
  <Carousel :slides="slides"></Carousel>
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
      slides: [],
    };
  },
  created() {
    (this.slides = [
      {
        id: 1,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1637193899campa%C3%B1as%20nuevas%20diferenciales%20Camilo_Mesa%20de%20trabajo%201%20copia%2020%20copy%202.png",
        href: "",
      },
      {
        id: 2,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1642779740Mesa%20de%20trabajo%201%20copia%20104%20%281%29.png",
        href: "",
      },
      {
        id: 3,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1642779226Dog-Days-con-tyc-l.png",
        href: "",
      },
      {
        id: 4,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1639579150concurso%20fin%20de%20a%C3%B1o%20BANNER%20%282%29%20%281%29.jpg",
        href: "",
      },
      {
        id: 5,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1641408181beneficios-Light-pg-Mailing-650x800.jpg",
        href: "",
      },
    ]),
      (this.categories = [
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
      ]);
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

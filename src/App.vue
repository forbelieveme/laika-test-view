<template>
  <Header :categories="categories" />
  <Carousel :slides="slides" />
  <Categories :categories="categories" />
  <Products :products="products" />
  <Footer :partners="partners" />
</template>

<script>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Carousel from "./components/Carousel.vue";
import Categories from "./components/Categories.vue";
import Products from "./components/Products.vue";

export default {
  name: "App",
  components: {
    Header,
    Footer,
    Carousel,
    Categories,
    Products,
  },
  data() {
    return {
      categories: [],
      slides: [],
      partners: [],
      products: [],
      hovered: false,
    };
  },
  methods: {
    async fetchProducts() {
      const res = await fetch("api/products");

      const data = await res.json();

      return data;
    },
  },
  async created() {
    (this.slides = [
      {
        id: 1,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1637193899campa%C3%B1as%20nuevas%20diferenciales%20Camilo_Mesa%20de%20trabajo%201%20copia%2020%20copy%202.png",
        href: "#",
      },
      {
        id: 2,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1642779740Mesa%20de%20trabajo%201%20copia%20104%20%281%29.png",
        href: "#",
      },
      {
        id: 3,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1642779226Dog-Days-con-tyc-l.png",
        href: "#",
      },
      {
        id: 4,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1639579150concurso%20fin%20de%20a%C3%B1o%20BANNER%20%282%29%20%281%29.jpg",
        href: "#",
      },
      {
        id: 5,
        url: "https://laikapp.s3.amazonaws.com/dev_images_banners/1641408181beneficios-Light-pg-Mailing-650x800.jpg",
        href: "#",
      },
    ]),
      (this.products = await this.fetchProducts()),
      (this.categories = [
        {
          id: 1,
          title: "Alimento",
          url: "#",
          icon: "apple-alt",
        },
        {
          id: 2,
          title: "Snacks",
          url: "#",
          icon: "bone",
        },
        {
          id: 3,
          title: "Farmapet",
          url: "#",
          icon: "prescription-bottle-alt",
        },
        {
          id: 4,
          title: "Cuidado e Higiene",
          url: "#",
          icon: "pump-medical",
        },
        {
          id: 5,
          title: "Juguetes",
          url: "#",
          icon: "baseball-ball",
        },
        {
          id: 6,
          title: "Accesorios",
          url: "#",
          icon: "life-ring",
        },
        {
          id: 7,
          title: "Para PetLovers",
          url: "#",
          icon: "heart",
        },
      ]),
      (this.partners = [
        {
          id: 1,
          href: "#",
          name: "american",
          url: "https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/American_Express_logo_%282018%29.svg/601px-American_Express_logo_%282018%29.svg.png",
        },
        {
          id: 2,
          href: "#",
          name: "visa",
          url: "https://cdn.visa.com/v2/assets/images/logos/visa/blue/logo.png",
        },
        {
          id: 3,
          href: "#",
          name: "mastercard",
          url: "https://brand.mastercard.com/content/dam/mccom/brandcenter/thumbnails/mastercard_circles_92px_2x.png",
        },
        {
          id: 4,
          href: "#",
          name: "mercadopago",
          url: "https://http2.mlstatic.com/frontend-assets/ui-navigation/5.18.5/mercadopago/logo__large@2x.png",
        },
        {
          id: 5,
          href: "#",
          name: "huawieApp",
          url: "https://laika.com.co/assets/huaweiGallery.png",
        },
        {
          id: 6,
          href: "#",
          name: "googleApp",
          url: "https://laika.com.co/assets/GOOGLEP.png",
        },
        {
          id: 7,
          href: "#",
          name: "appStore",
          url: "https://laika.com.co/assets/APP.png",
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
}

.bg_purple {
  background-color: #603e85 !important;
}
.color_purple {
  color: #603e85 !important;
}

.w-40 {
  width: 40% !important;
}

.text_decoration_general {
  text-decoration: none !important;
}

.foo-hover {
  color: red;
}

.border_purple {
  border-color: #603e85 !important;
}
</style>

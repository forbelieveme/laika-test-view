<template>
  <div class="mx-lg-5"> 
    <h3 class="pt-2 text-lg-start fw-bolder mx-2">Productos</h3>
    <div class="container overflow-scroll no_scroll">
      <div class="row d-flex justify-content-start product_width">
        <div :key="product.id" v-for="product in products" class="col-auto">
          <Product :product="product" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Product from "./Product.vue";

export default {
  name: "Products",
  components: {
    Product,
  },
  props: {
    products: Array,
  },
};
</script>

<style scoped>
.product_width {
  width: 2600px;
}

/* Hide scrollbar for Chrome, Safari and Opera */
.no_scroll::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.no_scroll {
  -ms-overflow-style: none; /* IE and Edge */
  scrollbar-width: none; /* Firefox */
}
</style>
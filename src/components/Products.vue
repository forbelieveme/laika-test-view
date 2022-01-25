<template>
  <div class="container overflow-hidden">
    <div class="row d-flex justify-content-center product_width">
      <h3 class="pt-2">Productos</h3>
      <div :key="product.id" v-for="product in products" class="col-auto">
        <Product :product="product" />
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
</style>
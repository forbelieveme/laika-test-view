<template>
  <div class="card" style="width: 18rem">
    <img
      :src="product.filename"
      class="card-img-top img_card_products"
      alt="..."
    />
    <div class="card-body">
      <h5 class="card-title">Card title</h5>
      <p class="card-text">
        Some quick example text to build on the card title and make up the bulk
        of the card's content.
      </p>
      <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: {
    product: Object,
  },
};
</script>

<style scoped>
.img_card_products {
  width: auto !important;
  height: 190px;
}
</style>
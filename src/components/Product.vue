<template>
  <div class="card" style="width: 17rem">
    <img
      :src="product.filename"
      class="card-img-top img_card_products mb-3"
      alt="..."
    />
    <div class="card-body d-flex flex-column p-0">
      <h5 class="card-title d-flex justify-content-start ms-3">Card title</h5>
      <p class="card-text ms-3 text-start">
        Some quick example text to build on the card title and make up the bulk
        of the card's content.
      </p>
    </div>
    <a href="#" class="btn btn-primary col-12 m-0 mt-4">Go somewhere</a>
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
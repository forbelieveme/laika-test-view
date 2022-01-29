<template>
  <div class="mx-lg-5">
    <h3 class="pt-2 text-lg-start fw-bolder mx-2">Categorias</h3>
    <div class="row d-flex justify-content-center">
      <div
        :key="categorie.id"
        v-for="categorie in categories"
        class="col-12 col-lg-3"
      >
        <Categorie :categorie="categorie" class="col" />
      </div>
    </div>
  </div>
</template>

<script>
import Categorie from "./Categorie.vue";

export default {
  name: "Categories",
  props: {
    categories: Array,
  },
  components: {
    Categorie,
  },
};
</script>
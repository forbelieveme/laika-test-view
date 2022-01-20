<template>
  <div class="row">
    <div :key="categorie.id" v-for="categorie in categories" class="col-12 col-lg-3">
      <Categorie :categorie="categorie" class="col"></Categorie>
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
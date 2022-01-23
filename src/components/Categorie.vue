<template>
<!-- TODO -->
<!-- Editar los estilos de hover -->
  <div class="">
    <a
      :href="categorie.url"
      class="btn btn-categorie tn-lg col-11 mx-2 my-1"
      tabindex="-1"
      role="button"
      aria-disabled="true"
      ><font-awesome-icon :icon="['fas', categorie.icon]" /> {{ categorie.title }}</a
    >
  </div>
</template>

<script>
export default {
  name: "Categorie",
  props: { categorie: Object },
};
</script>

<style scoped>
.btn-categorie {
    color: #603e85;
    background-color: #fff;
    border-color: #603e85;
}
</style>
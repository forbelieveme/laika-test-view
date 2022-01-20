<template>
  <div class="categorie">
    <a
      :href="categorie.url"
      class="btn btn-primary btn-lg"
      tabindex="-1"
      role="button"
      aria-disabled="true"
      >{{ categorie.title }}</a
    >
  </div>
</template>

<script>
export default {
  name: "Categorie",
  props: { categorie: Object },
};
</script>
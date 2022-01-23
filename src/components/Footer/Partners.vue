<template>
  <div id="footer-convenios" class="col-12 mt-5 bg-light">
    <div class="row d-flex justify-content-evenly py-4">
      <div
        :key="partner.id"
        v-for="partner in partners"
        class="col-auto"
        :id="partner.name"
      >
        <a :href="partner.href"><img :src="partner.url" alt="" /> </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Partners",
  props: {
    partners: Array,
  },
};
</script>

<style scoped>
#footer-convenios img {
  width: 80px;
}
</style>
<template>
  <InfoNav></InfoNav>
  <div class="sticky-top">
    <MainNav></MainNav>
  </div>
  <SalesNav :categories="categories"></SalesNav>
</template>

<script>
import MainNav from "./Header/MainNav.vue";
import InfoNav from "./Header/InfoNav.vue";
import SalesNav from "./Header/SalesNav.vue";

export default {
  name: "Header",
  components: {
    MainNav,
    InfoNav,
    SalesNav,
  },
  props: {
    categories: Array,
  },
  methods: {},
};
</script>


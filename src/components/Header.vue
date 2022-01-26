<template>
  <InfoNav></InfoNav>
  <div class="sticky-top">
    <MainNav></MainNav>
    <SalesNav></SalesNav>
  </div>
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
};
</script>


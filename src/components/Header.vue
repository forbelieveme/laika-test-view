<template>
  <InfoNav></InfoNav>
  <MainNav class="sticky-top"></MainNav>
</template>

<script>
import MainNav from "./Header/MainNav.vue";
import InfoNav from "./Header/InfoNav.vue";

export default {
  name: "Header",
  components: {
    MainNav,
    InfoNav,
  },
};
</script>


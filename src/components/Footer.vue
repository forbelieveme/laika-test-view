<template>
  <footer class="pt-2 container-fluid mt-5">
    <div class="row justify-content-center">
      <Brand />

      <Info />
      <!-- TODO -->
      <!-- Insertar un arreglo con la informacion  -->
      <!-- de los elementos del acordeon -->
      <Accordion />
      <Accordion />
      <Accordion />

      <div class="col-12 col-lg-2">
        <form>
          <h5>Subscribe to our newsletter</h5>
          <p>Monthly digest of whats new and exciting from us.</p>
          <div class="d-flex w-100 gap-2">
            <label for="newsletter1" class="visually-hidden"
              >Email address</label
            >
            <input
              id="newsletter1"
              type="text"
              class="form-control"
              placeholder="Email address"
            />
            <button class="btn btn-primary" type="button">Subscribe</button>
          </div>
        </form>
      </div>
    </div>

    <Partners :partners="partners" />
  </footer>
</template>

<script>
import Partners from "./Footer/Partners.vue";
import Accordion from "./Footer/Accordion.vue";
import Brand from "./Footer/Brand.vue";
import Info from "./Footer/Info.vue";

export default {
  name: "Footer",
  props: {
    title: String,
    partners: Array,
  },
  components: {
    Partners,
    Accordion,
    Brand,
    Info,
  },
};
</script>

<style scoped>
</style>
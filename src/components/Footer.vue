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

      <div class="col-12 col-lg-2 mt-5 mt-lg-0">
        <form>
          <h5>Subscribe to our newsletter</h5>
          <p>Monthly digest of whats new and exciting from us.</p>
          <div class="d-flex w-100 gap-2">
            <div
              class="
                input-group
                col-12 col-md-12 col-lg-12
                offset-xl-1
                col-xl-7
                p-0
              "
            >
              <input
                type="text"
                class="autocomplete_search_style form-control border-end-0"
                name="autocomplete_search"
                id="autocomplete_search"
                placeholder="¿Qué necesita tu mascota?"
              />
              <button
                type="button"
                class="btn border border-start-0"
              >
                <span
                  class=""
                  style="width: 30px; height: 25px"
                >
                  <font-awesome-icon icon="angle-right" />
                </span>
              </button>
            </div>
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
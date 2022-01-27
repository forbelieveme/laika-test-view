<template>
  <div class="accordion d-block d-xl-none mb-1" :id="'A' + data[0].btnName">
    <div class="accordion-item col-12 shadow-sm border-0">
      <h2 class="accordion-header" id="headingOne">
        <button
          class="accordion-button collapsed color_purple fw-bolder fs-7"
          type="button"
          data-bs-toggle="collapse"
          :data-bs-target="'#' + data[0].btnName"
          aria-expanded="true"
          :aria-controls="data[0].btnName"
          style="border-bottom: 0px solid white !important"
        >
          {{ data[0].title }}
        </button>
      </h2>
      <div
        :id="data[0].btnName"
        class="accordion-collapse collapse text-start"
        aria-labelledby="headingOne"
        :data-bs-parent="'#A' + data[0].btnName"
      >
        <div :key="x.id" v-for="x in data" class="card-body px-3 py-2">
          <a
            class="nav-link p-0 text-muted"
            href="https://laika.com.co/about_us/bog"
          >
            <span class="p_text_footer mb-1 fw-bolder color_purple">{{ x.text }}</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Accordion",
  props: {
    data: Array,
  },
};
</script>

<style scoped>
.accordion-button:not(.collapsed) {
  color: #603e85;
  background-color: #fff;
  box-shadow: none;
}

.accordion-button:focus {
  z-index: 3;
  border-color: transparent;
  outline: 0;
  box-shadow: 0 0 0 0.25rem transparent;
}
</style>
<template>
  <div class="accordion d-block d-sm-none mb-1" id="accordionExample">
    <div class="accordion-item col-12 mx-2">
      <h2 class="accordion-header" id="headingOne">
        <button
          class="accordion-button collapsed"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#collapseOne"
          aria-expanded="true"
          aria-controls="collapseOne"
          style="border-bottom: 0px solid white !important"
        >
          Accordion Item #1
        </button>
      </h2>
      <div
        id="collapseOne"
        class="accordion-collapse collapse"
        aria-labelledby="headingOne"
        data-bs-parent="#accordionExample"
      >
        <div class="card-body px-3 py-2">
          <a href="https://laika.com.co/about_us/bog">
            <h3 class="p_text_footer mb-1">Sobre Laika</h3>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Accordion",
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
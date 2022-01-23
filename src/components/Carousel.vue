<template>
  <div
    id="carouselExampleIndicators"
    class="carousel slide"
    data-bs-ride="carousel"
  >
    <div class="carousel-indicators">
      <button
        type="button"
        data-bs-target="#carouselExampleIndicators"
        data-bs-slide-to="0"
        class="active"
        aria-current="true"
        aria-label="Slide 1"
      ></button>
      <button
        :key="slide.id"
        v-for="(slide, index) in slides.slice(1)"
        type="button"
        data-bs-target="#carouselExampleIndicators"
        :data-bs-slide-to="index + 1"
        aria-label="Slide 2"
      ></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <a :href="slides[0].href">
          <img :src="slides[0].url" class="d-block w-100" alt="..." />
        </a>
      </div>
      <div
        :key="slide.id"
        v-for="slide in slides.slice(1)"
        class="carousel-item"
      >
        <a :href="slide.href">
          <img :src="slide.url" class="d-block w-100" :alt="slide.id" />
        </a>
      </div>
    </div>
    <button
      class="carousel-control-prev"
      type="button"
      data-bs-target="#carouselExampleIndicators"
      data-bs-slide="prev"
    >
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button
      class="carousel-control-next"
      type="button"
      data-bs-target="#carouselExampleIndicators"
      data-bs-slide="next"
    >
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</template>

<script>
export default {
  name: "Carousel",
  props: {
    slides: Array,
  },
};
</script>





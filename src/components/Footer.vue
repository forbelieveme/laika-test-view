<template>
  <footer class="pt-2">
    <div class="row">
      <!-- *********************** -->
      <!-- Hidden in small screens -->
      <!-- *********************** -->
      <div class="col-12 d-none d-sm-block">
        <h5>Section</h5>
        <ul class="nav flex-column">
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Home</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Features</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Pricing</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">FAQs</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">About</a>
          </li>
        </ul>
      </div>

      <div class="col-12 d-none d-sm-block">
        <h5>Section</h5>
        <ul class="nav flex-column">
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Home</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Features</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Pricing</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">FAQs</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">About</a>
          </li>
        </ul>
      </div>

      <div class="col-12 d-none d-sm-block">
        <h5>Section</h5>
        <ul class="nav flex-column">
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Home</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Features</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">Pricing</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">FAQs</a>
          </li>
          <li class="nav-item mb-2">
            <a href="#" class="nav-link p-0 text-muted">About</a>
          </li>
        </ul>
      </div>

      <!-- *********************** -->
      <!-- Hidden in small screens -->
      <!-- *********************** -->

      <Accordion class="d-block d-sm-none"/>

      <div class="col-12">
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

    <!-- *********************** -->
    <!-- Partners logos -->
    <!-- *********************** -->

    <Partners :partners="partners" />
    <!-- *********************** -->
    <!-- Partners logos -->
    <!-- *********************** -->
  </footer>
</template>

<script>
import Partners from "./Footer/Partners.vue";
import Accordion from "./Footer/Accordion.vue";

export default {
  name: "Footer",
  props: {
    title: String,
    partners: Array,
  },
  components: {
    Partners,
    Accordion,
  },
};
</script>

<style scoped>
</style>
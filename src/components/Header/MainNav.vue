<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg_purple">
    <div class="container-fluid">
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <a class="navbar-brand" href="#">
        <img
          src="https://laika.com.co/assets/home/LaikaMascotas.svg"
          alt=""
          width="30"
          height="24"
          class="d-inline-block align-text-top"
        />
      </a>

      <div
        class="
          input-group
          col-12 col-md-12 col-lg-12
          offset-xl-1
          col-xl-7
          p-0 p-0
        "
      >
        <input
          type="text"
          class="autocomplete_search_style placeholder form-control"
          name="autocomplete_search"
          id="autocomplete_search"
          placeholder="¿Qué necesita tu mascota?"
        />
        <img
          src="https://laika.com.co/assets/home/search_icon_mc.svg"
          id="btn_result_search"
          alt=""
          class="icon_search"
          style="visibility: visible"
        />
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "MainNav",
};
</script>

<style scoped>
.icon_search {
  right: 0;
}

.icon_close_searcher,
.icon_search {
  padding: 7px 10px;
  z-index: 10;
  cursor: pointer;
  color: #614186;
  position: absolute;
}

.autocomplete_search_style {
  /* padding-left: 45px !important; */
  border: 0 solid #ced4da !important;
  border-radius: 8px !important;
  z-index: 2;
}

.bg_purple {
  background-color: #603e85 !important;
}
</style>
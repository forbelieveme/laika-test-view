<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg_purple">
    <div class="container">
      <div class="d-flex w-100 row">
        <!-- ************** -->
        <!-- Boton de collapse -->
        <!-- ************** -->
        <button
          class="navbar-toggler col-1"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <!-- ************** -->
        <!-- Boton de collapse -->
        <!-- ************** -->

        <!-- ************** -->
        <!-- Logo -->
        <!-- ************** -->
        <a class="navbar-brand col-3 offset-4" href="#">
          <img
            src="https://laika.com.co/assets/home/LaikaMascotas.svg"
            alt=""
            width="30"
            height="24"
            class="d-inline-block align-text-top"
          />
        </a>
        <!-- ************** -->
        <!-- Logo -->
        <!-- ************** -->

        <!-- ************** -->
        <!-- Ubicacion -->
        <!-- ************** -->
        <div class="d-flex flex-row col-2">
          <div class="d-flex flex-column position-relative">
            <img
              src="https://i.pinimg.com/originals/50/a7/c2/50a7c209831660bce1c7b647281e4e0a.png"
              style="height: 15px; width: 35px"
            />
            <div class="text-white d-inline">
              <span>BOG</span>
            </div>
          </div>
          <span class="d-flex align-self-center">
            <div class="px-2">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="14.225"
                height="8.107"
                viewBox="0 0 14.225 8.107"
                style="height: 6px; top: 5px"
              >
                <g>
                  <path
                    fill="white"
                    d="M104.955 7.816l-6.116 6.116a1 1 0 1 1-1.409-1.409l5.412-5.412L97.43 1.7A1 1 0 0 1 98.839.292l6.116 6.116a1 1 0 0 1 0 1.408z"
                    transform="rotate(90 7.112 7.113) translate(-97.139)"
                  ></path>
                </g>
              </svg>
            </div>
          </span>
        </div>
        <!-- ************** -->
        <!-- Ubicacion -->
        <!-- ************** -->

        <!-- ************** -->
        <!-- Carro de compras -->
        <!-- ************** -->
        <div class="d-flex flex-row col-1 pl-4">
          <div>
            <div class="btn-group">
              <span
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
                class="cursor_pointer"
                ><div class="circle_bg_cart">
                  <img
                    data-src=" https://laika.com.co/assets/home/cart_mc.svg "
                    class="lazy vertical_at"
                    src=" https://laika.com.co/assets/home/cart_mc.svg "
                    style=""
                  />
                </div>
                <span class="badge badge_car rounded-circle">0</span></span
              >
            </div>
          </div>
        </div>
      </div>
      <!-- ************** -->
      <!-- Carro de compras -->
      <!-- ************** -->

      <!-- ************** -->
      <!-- Barra de busqueda -->
      <!-- ************** -->
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
          class="autocomplete_search_style form-control"
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
      <!-- ************** -->
      <!-- Barra de busqueda -->
      <!-- ************** -->
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

.badge_car {
  position: absolute;
  top: -7px !important;
  width: 18px;
  right: -7px;
  min-width: fit-content;
  height: 18px !important;
  background-color: #ff007a;
  color: #fff;
  font-size: 11px;
}
.rounded-circle {
  border-radius: 50% !important;
}
.badge {
  display: inline-block;
  padding: 0.25em 0.4em;
  font-size: 75%;
  font-weight: 700;
  line-height: 1;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: 0.25rem;
  transition: color 0.15s ease-in-out, background-color 0.15s ease-in-out,
    border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}
</style>
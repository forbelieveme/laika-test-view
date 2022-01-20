<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg_purple">
    <div class="container">
      <div class="d-flex justify-content-between w-100">
        <!-- ************** -->
        <!-- Boton de collapse -->
        <!-- ************** -->
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
        <!-- ************** -->
        <!-- Boton de collapse -->
        <!-- ************** -->

        <!-- ************** -->
        <!-- Logo -->
        <!-- ************** -->
        <a class="navbar-brand" href="#">
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
        <div class="d-flex flex-row">
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
        <div class="d-flex flex-row">
          <div id="cart_header" class="header_navbar_small_cart">
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
              <div
                class="dropdown-menu dropdown-menu-right mt-2 dropdown_cart"
                style="background: rgb(250, 250, 250)"
              >
                <div
                  class="dropdown-header text-right"
                  style="padding: 0px 1.5rem !important"
                >
                  <span
                    class="font_nova_bold color_purple"
                    style="font-size: 18px; cursor: pointer"
                    >X</span
                  >
                </div>
                <div class="dropdown-divider"></div>
                <div
                  class="ml-1 mr-1 p-3 font_causten_round_semi_bold_oblique"
                  style="max-height: 310px; overflow-y: auto"
                >
                  <div class="cart-checkout">
                    <p class="mb-0">El carrito está vacio</p>
                  </div>
                  <!---->
                </div>
                <div
                  class="
                    container_want_save_with_membership
                    mx-3
                    p-2
                    position-relative
                  "
                  style="display: none"
                >
                  <div class="d-flex">
                    <img
                      src="https://laika.com.co/assets/imgs_landing_member/crown.svg"
                      alt=""
                      class="mr-2"
                    />
                    <div
                      class="font-12 mr-2 align-self-center"
                      style="display: none"
                    >
                      ¿Quieres ahorrar <span class="text-success">$0</span>?
                    </div>
                    <div class="font-12 mr-2 align-self-center">
                      ¿Quieres ahorrar en tus pedidos?
                    </div>
                    <button class="position-absolute btn btn_want_save font-10">
                      Ahorra
                    </button>
                  </div>
                </div>
                <div class="dropdown-divider"></div>
                <div class="container_without_delivery_free">
                  <div class="text-center btn_checkout_cart">
                    <a
                      type="button"
                      class="btn bg_purple text-white shadow rounded disabled"
                      style="appearance: none !important"
                      ><div class="text-left">
                        Continuar al Checkout
                        <span class="text-right cart_price_span"
                          >$<span id="price_cart_checkout">0</span></span
                        >
                      </div></a
                    >
                  </div>
                </div>
              </div>
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
    top: -7px!important;
    width: 18px;
    right: -7px;
    min-width: fit-content;
    height: 18px!important;
    background-color: #ff007a;
    color: #fff;
    font-size: 11px;
}
.rounded-circle {
    border-radius: 50%!important;
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
    transition: color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;
}
</style>
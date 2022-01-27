<template>
  <nav class="navbar navbar-dark bg_purple d-block d-xl-none sticky-top">
    <div class="container-fluid">
      <div class="d-flex flex-column w-100 mx-2">
        <div class="d-flex flex-row justify-content-between">
          <div class="d-flex justify-content-start">
            <button class="navbar-toggler" type="button" @click="menuToggle">
              <span class="navbar-toggler-icon"></span>
            </button>
          </div>
          <div class="d-flex justify-content-center">
            <a class="navbar-brand" href="#">
              <img
                src="https://laika.com.co/assets/home/LaikaMascotas.svg"
                alt=""
                width="30"
                height="24"
                class="d-inline-block align-text-top"
              />
            </a>
          </div>
          <div class="d-flex justify-content-between">
            <div class="d-flex flex-row me-2">
              <div class="d-flex flex-column me-1">
                <img
                  src="https://i.pinimg.com/originals/50/a7/c2/50a7c209831660bce1c7b647281e4e0a.png"
                  style="height: 15px; width: 35px"
                />
                <div class="text-white d-inline">
                  <span>BOG</span>
                </div>
              </div>
              <span class="d-flex align-self-center">
                <font-awesome-icon
                  :icon="['fas', 'chevron-down']"
                  class="align-self-center text-white"
                />
              </span>
            </div>
            <div class="btn-group align-self-center">
              <span
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >
                <div>
                  <img
                    data-src=" https://laika.com.co/assets/home/cart_mc.svg "
                    class="lazy"
                    src=" https://laika.com.co/assets/home/cart_mc.svg "
                    style=""
                  />
                </div>
                <span class="badge badge_car rounded-circle">0</span>
              </span>
            </div>
          </div>
        </div>
        <div class="d-flex mt-2">
          <div class="input-group">
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
        </div>
      </div>
    </div>
    <div
      class="position-absolute start-0 w-100 offcanvas_2 offcanvas_start"
      :class="{ show: isActive }"
      style="visibility: visible"
    >
      HolaHolaHolaHola
    </div>
  </nav>

  <!-- * -->
  <!-- * -->
  <!-- * -->
  <!-- * -->
  <!-- * -->

  <nav class="navbar bg_purple d-none d-xl-block sticky-top">
    <div class="container-fluid">
      <div class="d-flex flex-row w-100 my-3">
        <div class="d-flex justify-content-start ms-5">
          <a class="navbar-brand me-5" href="#">
            <img
              src="https://laika.com.co/assets/home/LaikaMascotas.svg"
              alt=""
              width="38"
              height="32"
            />
          </a>
          <div class="input-group p-0 search_width">
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
          <div class="d-flex flex-row">
            <div class="ms-3 align-self-center">
              <img
                src="https://i.pinimg.com/originals/50/a7/c2/50a7c209831660bce1c7b647281e4e0a.png"
                style="height: 30px; width: 50px"
              />
            </div>
            <div class="text-white align-self-center">
              <span>BOG</span>
            </div>
            <!-- TODO -->
            <!-- insertar icono fontwaesome -->
          </div>
        </div>
        <div class="d-flex justify-content-end ms-auto me-5">
          <span class="text-white text-left mx-3 align-self-center fs-5">
            <!-- TODO -->
            <!-- insertar el fontawsom de usuario -->
            <img
              class="lazy"
              data-src="https://laika.com.co/assets/home/truck_mc.svg"
              src="https://laika.com.co/assets/home/truck_mc.svg"
              style=""
            />
            Mi cuenta
          </span>
          <div class="btn-group align-self-center">
            <span
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
              class="cursor_pointer"
            >
              <div class="circle_bg_cart">
                <img
                  data-src=" https://laika.com.co/assets/home/cart_mc.svg "
                  class="lazy vertical_at"
                  src=" https://laika.com.co/assets/home/cart_mc.svg "
                  style=""
                />
              </div>
              <span class="badge badge_car rounded-circle">0</span>
            </span>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "MainNav",
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    menuToggle(event) {
      // `this` inside methods points to the current active instance
      this.isActive = !this.isActive;
      // console.log(event.fromElement.id);
      // `event` is the native DOM event
      if (event.type === "mouseenter") {
        this.isActive = !this.isActive;
      } else if (event.type === "mouseleave") {
        this.isActive = !this.isActive;
      }
    },
  },
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

.search_width {
  min-width: 40vw;
}

.offcanvas_start {
  width: 100vw;
  border-right: 1px solid rgba(0, 0, 0, 0.2);
  transform: translateX(-100%);
}

.offcanvas_2 {
  z-index: 0;
  display: flex;
  z-index: 1045;
  flex-direction: column;
  max-width: 100%;
  height: 100vh;
  visibility: hidden;
  background-color: #fff;
  background-clip: padding-box;
  outline: 0;
  transition: transform 0.3s ease-in-out;
}

.box {
  border: 2px red dotted;
}

.offcanvas_2.show {
  transform: none;
}
</style>
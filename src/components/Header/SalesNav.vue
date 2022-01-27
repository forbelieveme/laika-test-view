<template>
  <div
    class="
      d-xs-flex d-sm-none d-md-none d-xl-none
      col-12
      row
      mx-auto
      py-2
      bg-white
      justify-content-center
    "
  >
    <a href="#" class="col-4 offset-2">
      <div class="" style="cursor: pointer; background: #603e85; color: #fff">
        <span class="ml-2" style="background: #603e85; color: #fff">
          Perro
        </span>
        <span class="text-left text-white mr-1 ml-1">
          <img
            width="30"
            src="https://laika.com.co/assets/home/dog_mc.svg "
            alt="Colombia "
          />
        </span>
      </div>
    </a>
    <a href="#" class="col-4">
      <div class="ml-2" style="cursor: pointer">
        <span class="ml-2" style=""> Gato </span>
        <span class="text-left text-white mr-1 ml-1">
          <img
            width="30"
            class="no_decoration_links"
            src="https://laika.com.co/assets/home/cat_mc_s.svg "
            alt="Colombia "
          />
        </span>
      </div>
    </a>
    <div
      id="header_pets_dog_cat_resp"
      class="
        px-0
        d-sm-flex d-xl-none
        row
        col-12
        mx-auto
        py-2
        bg-white
        justify-content-center
      "
    >
      <div>
        <input type="hidden" id="clevertap_membership" />
        <img
          data-src=" https://lkdev-webcol.laika.com.co/assets/laika_vetcare/membership_logo.png "
          src=" https://lkdev-webcol.laika.com.co/assets/laika_vetcare/membership_logo.png "
          class="cursor_pointer lazy br-8 mx-2"
          style=""
        />
      </div>
    </div>
  </div>
<!-- * -->
<!-- * -->
<!-- * -->
<!-- * -->
<!-- * -->

  <div class="navbar bg-white d-none d-xl-block sticky-top">
    <div class="container-fluid">
      <div class="d-flex flex-row w-100 justify-content-between">
        <div class="d-flex w-40 justify-content-center">
          <div
            id="menu_perro"
            aria-haspopup="true"
            aria-expanded="false"
            class="mx-3 align-self-center position-relative"
            @mouseenter="menuToggle"
            @mouseleave="menuToggle"
          >
            <span class="text-left text-white">
              <img
                width="30"
                src="https://laika.com.co/assets/home/dog_mc.svg "
              />
              <span id="active-dog" class="color_purple align-self-center">
                Compra para perro
              </span>
              <img
                src="https://laika.com.co/assets/punto_de_flecha_a_la_derecha_1.svg"
                alt=""
                class=""
                style="height: 11px"
              />
            </span>

            <div
              class="position-absolute start-0 hidden_menu_width"
              :class="{ 'visually-hidden': isActive }"
              @mouseenter="menuToggle"
            >
              <div class="d-flex flex-row w-100 bg-white">
                <div class="d-flex flex-column w-100 bg-white">
                  <div class="list-group list-group-flush">
                    <button
                      :key="categorie.id"
                      v-for="categorie in categories"
                      class="
                        list-group-item list-group-item-action
                        d-flex
                        justify-content-between
                      "
                    >
                      <div class="">
                        <a
                          :href="categorie.url"
                          class="btn btn-categorie tn-lg my-1 fs_categories"
                          tabindex="-1"
                          role="button"
                          aria-disabled="true"
                        >
                          <font-awesome-icon :icon="['fas', categorie.icon]" />
                          {{ categorie.title }}
                        </a>
                      </div>
                      <font-awesome-icon
                        :icon="['fas', 'chevron-right']"
                        class="align-self-center"
                      />
                    </button>
                  </div>
                </div>
                <div class="d-flex w-100 bg-white justify-content-end">
                  <img
                    class="img_width"
                    src="https://i.pinimg.com/736x/6a/68/1b/6a681bfc979f63e3759d2a59ce3ea298.jpg"
                  />
                </div>
              </div>
            </div>
          </div>
          <div
            id="menu_gato"
            aria-haspopup="true"
            aria-expanded="false"
            class="mx-3 align-self-center"
          >
            <span class="text-left text-white">
              <img
                width="30"
                src="https://laika.com.co/assets/home/cat_mc_s.svg"
              />
              <span id="active-cat" class="color_purple">
                Compra para gato
              </span>
              <img
                src="https://laika.com.co/assets/punto_de_flecha_a_la_derecha_1.svg"
                alt=""
                class=""
                style="height: 11px"
              />
            </span>
          </div>
        </div>
        <!-- *************** -->
        <!-- *************** -->
        <!-- *************** -->
        <div class="d-flex justify-content-evenly w-40">
          <div
            id="menu_ofertas"
            aria-haspopup="true"
            aria-expanded="false"
            class="align-self-center"
          >
            <span class="text-left text-white">
              <span id="active-ofertas" class="color_purple"> Ofertas </span>
              <img
                src="https://laika.com.co/assets/punto_de_flecha_a_la_derecha_1.svg"
                alt=""
                class=""
                style="height: 11px"
              />
            </span>
          </div>
          <div
            id="menu_servicios"
            aria-haspopup="true"
            aria-expanded="false"
            class="align-self-center"
          >
            <span class="text-left text-white">
              <span id="active-servicios" class="color_purple">
                Servicios
              </span>
              <img
                src="https://laika.com.co/assets/punto_de_flecha_a_la_derecha_1.svg"
                alt=""
                class=""
                style="height: 11px"
              />
            </span>
          </div>
          <div
            aria-haspopup="true"
            aria-expanded="false"
            class="align-self-center"
          >
            <span class="text-left">
              <a href="#">
                <span id="active-servicios" class="color_purple text-muted">
                  Blog
                </span>
              </a>
            </span>
          </div>
        </div>
        <!-- ************** -->
        <!-- ************** -->
        <!-- ************** -->
        <div class="d-flex justify-content-end ms-auto me-5">
          <div class="">
            <a href="#" class="pe-auto">
              <img
                width="160"
                src=" https://laika.com.co/assets/laika_vetcare/membership_logo.png "
              />
            </a>
          </div>
          <div class="">
            <a href="#" class="pe-auto">
              <img
                width="160"
                src=" https://laika.com.co/assets/laika_vetcare/membership_logo.png "
              />
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SalesNav",
  props: {
    categories: Array,
  },
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    menuToggle(event) {
      // `this` inside methods points to the current active instance
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
.hidden_menu_width {
  width: 50vw;
}

.list-group-item {
  position: relative;
  display: block;
  color: #212529;
  text-decoration: none;
  background-color: #fff;
}

a {
  color: #603e85;
  background-color: #fff;
  border: 0 !important;
}

.fs_categories {
  font-size: 1.3rem;
}

.img_width {
  display: block;
  max-width: 230px;
  max-height: 480px;
  width: auto;
  height: auto;
}
</style>
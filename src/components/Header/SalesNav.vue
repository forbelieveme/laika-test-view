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

  <div class="navbar bg-white d-none d-xl-block">
    <div class="container-fluid">
      <div class="d-flex flex-row w-100 justify-content-between">
        <div class="d-flex w-40 justify-content-center">
          <div
            id="menu_perro"
            aria-haspopup="true"
            aria-expanded="false"
            class="mx-3 align-self-center"
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
};
</script>

<style scoped>
</style>
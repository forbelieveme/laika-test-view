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
      <div
        class=""
        style="cursor: pointer; background: #603e85; color: #fff"
      >
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
      <div class=" ml-2" style="cursor: pointer">
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
</template>

<script>
export default {
  name: "SalesNav",
};
</script>

<style scoped>

</style>
<template>
  <div class="navbar bg-dark d-none d-lg-block">
    <div class="container-fluid">
      <div class="d-flex flex-row w-100">
        <div class="d-flex justify-content-start ms-5 me-auto">
          <span class="text-white text-left pe-3 border-end fonts_11">
            <img
              class="lazy"
              data-src=" https://laika.com.co/assets/home/secure_mc.svg "
              src=" https://laika.com.co/assets/home/secure_mc.svg "
              style=""
            />
            Compras seguras online
          </span>
          <span class="text-white text-left ms-3 pe-3 border-end fonts_11">
            <img
              class="lazy"
              data-src="https://laika.com.co/assets/home/wallet_mc.svg"
              src="https://laika.com.co/assets/home/wallet_mc.svg"
              style=""
            />Pago contra entrega
          </span>
          <span class="text-white text-left ms-3 fonts_11">
            <img
              class="lazy"
              data-src="https://laika.com.co/assets/home/truck_mc.svg"
              src="https://laika.com.co/assets/home/truck_mc.svg"
              style=""
            />
            Entregas el mismo día
          </span>
        </div>
        <div class="d-flex justify-content-end me-5">
          <span
            class="
              text-white text-left
              pe-3
              border-end
              fonts_11
              align-self-center
            "
          >
            Llamanos +573102563989
          </span>
          <span class="text-white text-left ms-3 fonts_11 align-self-center"
            >Escribenos
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InfoNav",
};
</script>

<style scoped>
.fonts_11 {
  font-size: 11px;
}
</style>
<template>
  <div class="card" style="width: 17rem">
    <img
      :src="product.filename"
      class="card-img-top img_card_products mb-3"
      alt="..."
    />
    <div class="card-body d-flex flex-column p-0">
      <h5 class="card-title text-start ms-3">Card title</h5>
      <div class="d-flex flex-column ms-3">
        <div class="d-flex justify-content-start">
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="d-flex justify-content-start flex-row">
          <span class="align-self-center">$18.991</span>
          <div class="d-flex flex-column">
            <span>Antes</span>
            <strike class="font-11"> $19.990 </strike>
          </div>
        </div>
        <div class="d-flex justify-content-start flex-row">
          <span class="align-self-center">$16.992 </span>
          <div class="d-flex flex-column">
            <img
              width="80"
              data-src="https://laika.com.co/assets/laikamemeber.svg"
              class=""
              src="https://laika.com.co/assets/laikamemeber.svg"
              style=""
            />
            <button class="w-100 fs-6">ADQUIÉRELA YA</button>
          </div>
        </div>
      </div>
      <!-- * -->
      <!-- * -->
      <!-- * -->
      <!-- * -->
      <p class="heigh_container_info_cards d-flex justify-content-start ms-3">
        <span id="price_products_dog_1927">
          <span id="price_dog_1927" class="mr-1 ms-3">$18.991</span>
          <span class="text_old_product">
            <span>Antes</span> <br />
            <strike id="price_old_dog_1927" class="text_old_price font-11">
              $19.990
            </strike>
          </span>
          <span class="row m-0 pt-1 mt-1 line_throught_info_cards_top">
            <span class="mr-1 color_laika_member font-20">
              <span class="mr-2 dog_price_laika_member_1927">$16.992 </span>
            </span>
            <span class="btn_container_laika_member">
              <img
                width="80"
                data-src="https://laika.com.co/assets/laikamemeber.svg"
                class="ml-1 mb-1 lazy"
                src="https://laika.com.co/assets/laikamemeber.svg"
                style=""
              />
              <button class="font-12 btn_member btn_laika_member_cards w-25">
                ADQUIÉRELA YA
              </button>
            </span>
          </span>
        </span>
        <span id="txt_out_of_stock_dog_1927">
          <span id="out_of_stock_supplier" class="txt_out_of_stock"></span>
        </span>
      </p>
    </div>
    <a href="#" class="btn btn-primary col-12 m-0 mt-4">Go somewhere</a>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: {
    product: Object,
  },
};
</script>

<style scoped>
.img_card_products {
  width: auto !important;
  height: 190px;
}

.text_old_product {
  color: #747474;
  font-size: 10px;
  font-family: Causten Round Semi Bold Oblique;
  position: absolute;
}

.text_old_price {
  color: #747474;
  font-size: 14px;
  font-family: Causten Round Semi Bold Oblique;
}

.line_throught_info_cards_top {
  border-top: 1px solid #f2f2f2;
}

.font-11 {
  font-size: 11px;
}

.color_laika_member {
  color: #ac0000;
}

.font-20 {
  font-size: 20px;
}

.btn_container_laika_member {
  display: grid;
}

.btn_member {
  border-radius: 5px;
  background: #ffb100;
  background: linear-gradient(0deg, #ffb100 0, #ffcb24 100%);
  font-family: Causten Round Extra Bold Oblique !important;
  color: #1f033e;
  font-size: 12px;
}

.btn_laika_member_cards {
  padding: 4px 0;
  border: 0;
  font-size: 8px;
}

.heigh_container_info_cards {
  position: relative;
  height: 80px;
  color: #ac0000;
  font-size: 20px;
  font-family: Causten Round Semi Bold Oblique;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
</style>
<template>
  <div class="card" style="width: 17rem">
    <img
      :src="product.filename"
      class="card-img-top img_card_products mb-3"
      alt="..."
    />
    <div class="card-body d-flex flex-column p-0">
      <h5 class="card-title text-start ms-3">Card title</h5>
      <div class="d-flex flex-column">
        <div class="d-flex justify-content-start ms-3">
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
          <font-awesome-icon :icon="['fas', 'star']" />
        </div>
        <div class="d-flex justify-content-start flex-row ms-3">
          <span class="align-self-center price_big">$18.991</span>
          <div class="d-flex flex-column">
            <span class="text_old_product">Antes</span>
            <strike class="text_old_price"> $19.990 </strike>
          </div>
        </div>
        <div
          class="
            d-flex
            justify-content-start
            flex-row
            line_throught_info_cards_top
            ms-3
          "
        >
          <span class="align-self-center price_big">$16.992 </span>
          <div class="d-flex flex-column">
            <img
              width="80"
              data-src="https://laika.com.co/assets/laikamemeber.svg"
              class=""
              src="https://laika.com.co/assets/laikamemeber.svg"
              style=""
            />
            <button class="w-100 btn_member btn_laika_member_cards">
              ADQUIÉRELA YA
            </button>
          </div>
        </div>
        <a href="#" class="btn btn-primary col-12 m-0 mt-4">Go somewhere</a>
      </div>
    </div>
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
}

.text_old_price {
  color: #747474;
  font-size: 11px;
  font-family: Causten Round Semi Bold Oblique;
}

.line_throught_info_cards_top {
  border-top: 1px solid #f2f2f2;
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

.price_big {
  color: #ac0000;
  font-size: 20px;
  font-family: Causten Round Semi Bold Oblique;
}
</style>
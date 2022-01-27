<template>
  <footer class="pt-2 container-fluid mt-5">
    <div class="row justify-content-center">
      <Brand />

      <Info />
      <!-- TODO -->
      <!-- Insertar un arreglo con la informacion  -->
      <!-- de los elementos del acordeon -->
      <Accordion :data="links.acerca" />
      <Accordion :data="links.interes" />
      <Accordion :data="links.informacion" />

      <div
        class="
          col-12 col-lg-2
          mt-5 mt-lg-0
          text-start
          color_purple
          fw-bolder
          d-none d-xl-block
        "
      >
        <form>
          <h5 class="fw-bolder">SUSCRÍBETE</h5>
          <p>Recibe noticias y promociones al instante.</p>
          <div class="d-flex w-100 gap-2 justify-content-start">
            <div class="input-group col-12 col-md-12 col-lg-12 col-xl-7 p-0">
              <input
                type="text"
                class="
                  autocomplete_search_style
                  form-control
                  border_purple border-end-0
                "
                name="autocomplete_search"
                id="autocomplete_search"
                placeholder="¿Qué necesita tu mascota?"
              />
              <button
                type="button"
                class="btn border border-start-0 color_purple border_purple"
              >
                <span class="" style="width: 30px; height: 25px">
                  <font-awesome-icon icon="angle-right" />
                </span>
              </button>
            </div>
          </div>
        </form>
      </div>
    </div>

    <Partners :partners="partners" />
  </footer>
</template>

<script>
import Partners from "./Footer/Partners.vue";
import Accordion from "./Footer/Accordion.vue";
import Brand from "./Footer/Brand.vue";
import Info from "./Footer/Info.vue";

export default {
  name: "Footer",
  props: {
    title: String,
    partners: Array,
  },
  components: {
    Partners,
    Accordion,
    Brand,
    Info,
  },
  data() {
    return {
      links: {},
    };
  },
  created() {
    this.links = {
      acerca: [
        {
          id: 1,
          url: "#",
          text: "Sobre Laika",
          btnName: "primer_acc",
          title: "ACERCA DE LAIKA",
        },
        { id: 2, url: "#", text: "Servicios" },
        { id: 3, url: "#", text: "Trabaja con nosotros" },
        { id: 4, url: "#", text: "Blog" },
        { id: 5, url: "#", text: "Términos y condiciones" },
      ],
      interes: [
        {
          id: 1,
          url: "#",
          text: "Preguntas frecuentes",
          btnName: "segundo_acc",
          title: "LINKS DE INTERÉS",
        },
        { id: 2, url: "#", text: "¿Cómo comprar en Laika?" },
        { id: 3, url: "#", text: "Política de Privacidad" },
        { id: 4, url: "#", text: "Contáctanos" },
        { id: 5, url: "#", text: "Políticas de Entrega" },
      ],
      informacion: [
        {
          id: 1,
          url: "#",
          text: "Teléfono: +573009108496",
          btnName: "tercer_acc",
          title: "INFORMACIÓN",
        },
        { id: 2, url: "#", text: "servicioclientes@laika.com.co" },
        { id: 3, url: "#", text: "Bogotá D.C., Colombia" },
      ],
    };
  },
};
</script>

<style scoped>
</style>


Teléfono: +573009108496
servicioclientes@laika.com.co
Bogotá D.C., Colombia


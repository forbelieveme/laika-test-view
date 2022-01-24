<template>
  <div class="col-md-4 col-lg-2 text-center">
    <span>
      <img
        class="ml-2 text-right img-fluid img_laika_footer lazy"
        data-src="https://laika.com.co/assets/LAIKA.png  "
        src="https://laika.com.co/assets/LAIKA.png  "
        style=""
      />
      <p class="ml-0 ml-md-2 mt-2 p_img_laika_footer mb-0">Síguenos en:</p>
      <p class="ml-0 ml-md-1">
        <span class="filter-contrast-1">
          <a
            class="text_decoration_general"
            href="https://www.youtube.com/watch?v=gchln4oix68"
          >
            <font-awesome-icon
              :icon="['fab', 'facebook']"
              size="2x"
              style="color: #603e85"
            />
          </a>
        </span>
        <span class="filter-contrast-1">
          <a
            class="text_decoration_general"
            href="https://www.instagram.com/laikamascotas/?hl=es-la"
          >
            <font-awesome-icon
              :icon="['fab', 'youtube']"
              size="2x"
              style="color: #603e85"
            />
          </a>
        </span>
        <span class="filter-contrast-1">
          <a
            class="text_decoration_general"
            href="https://es-la.facebook.com/LaikaUniverso/"
          >
            <font-awesome-icon
              :icon="['fab', 'instagram']"
              size="2x"
              style="color: #603e85"
            />
          </a>
        </span>
      </p>
    </span>
  </div>
</template>

<script>
export default {
  name: "Brand",
};
</script>
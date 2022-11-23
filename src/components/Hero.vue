<template>
  <div class="heroBlock">
    <v-carousel hide-delimiters>
      <v-carousel-item v-for="(item, i) in items" :key="i">
        <v-img :src="item.src" aspect-ratio="1.77"></v-img>
        <!-- <v-row class="fill-height" align="center" justify="center">
          <div class="text-h1">Slide {{ i + 1 }}</div>
        </v-row> -->
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<script>
export default {
  name: "Hero-component",

  data() {
    return {
      items: [
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/sky.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/bird.jpg",
        },
        {
          src: "https://cdn.vuetifyjs.com/images/carousel/planet.jpg",
        },
      ],
    };
  },
};
</script>

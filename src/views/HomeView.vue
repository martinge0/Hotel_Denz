<template>
  <v-content>
    <Hero />
    <Gallery />
    <Rooms />
  </v-content>
</template>

<script>
import Hero from "../components/Hero";
import Gallery from "../components/Gallery";
import Rooms from "../components/Rooms";
export default {
  name: "Home-page",

  components: {
    Hero,
    Gallery,
    Rooms,
  },
};
</script>

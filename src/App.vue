<template>
  <v-app>
    <v-app-bar app color="#FFFFFF" flat>
      <Header />
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import Header from "../src/components/Header";
export default {
  name: "App",
  components: {
    Header,
  },

  data: () => ({
    //
  }),
};
</script>

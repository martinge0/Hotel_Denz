<template>
  <v-container>
    <v-toolbar flat>
      <v-toolbar-title>Hotel DENZ</v-toolbar-title>

      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn text v-show="$vuetify.breakpoint.smAndUp">Начало</v-btn>

        <v-btn text v-show="$vuetify.breakpoint.smAndUp">За нас</v-btn>

        <v-btn text v-show="$vuetify.breakpoint.smAndUp">Контакти</v-btn>
        <v-app-bar-nav-icon
          v-show="!$vuetify.breakpoint.smAndUp"
          @click.stop="drawer = !drawer"
        >
        </v-app-bar-nav-icon>
      </v-toolbar-items>
    </v-toolbar>
  </v-container>
</template>

<script>
export default {
  name: "Header-component",

  data: () => ({
    drawer: false,
    group: null,
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>

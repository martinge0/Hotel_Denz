<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Варианти за настаняване</h2>
      <v-row>
        <v-col cols="12" md="4" v-for="item in items" :key="item.id">
          <v-card class="mx-auto" max-width="400">
            <v-img class="white--text align-end" height="200px" :src="item.src">
              <v-card-title>{{ item.title }}</v-card-title>
            </v-img>

            <v-card-subtitle class="pb-0">{{ item.subtitle }}</v-card-subtitle>

            <v-card-text class="text--primary">
              <div>{{ item.description }}</div>
            </v-card-text>

            <v-card-actions>
              <v-btn color="orange" text> Разгледай </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Rooms-component",

  data: () => ({
    items: [
      {
        id: 1,
        title: "Апартамент с изглед към градината",
        subtitle: "Капацитет 5 човека",
        description:
          "Апатаментът се състои от всекидневна с кухненски бокс и спалня. В спалнята има легло Кингсайз и разтегателен фотьойл. Във всекидневната има разтегателен диван, маса за хранене, столове, хладилник и телевизор. ",
        src: require("../assets/rooms/Apartament_1/Hol1.jpg"),
      },
      {
        id: 2,
        title: "Christmas tales to read",
        subtitle: "2,000 miles of wonder",
        description:
          "Sea ad habemus assueverit, omnes platonem convenire sit et, at integre pericula quo. Facete adolescens definitionem cu qui, in putant aliquid fierent ius.",
        src: require("../assets/rooms/Apartament_2/Kuhnia2.jpg"),
      },
      {
        id: 3,
        title: "20 movies not to miss in 2020",
        subtitle: "3,000 miles of wonder",
        description:
          "Aliquam albucius mei ei, debitis torquatos et pro, eos natum scribentur no. Putant verear constituto te qui. Adolescens persequeris vim ei. Vel nullam reprimique te.",
        src: require("../assets/rooms/DvoinaStaia/2.jpg"),
      },
    ],
  }),
};
</script>

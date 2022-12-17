<template>
  <v-content class="product">
    <RegistrationForm />
  </v-content>
</template>

<script>
import RegistrationForm from "../components/RegistrationForm";
export default {
  name: "Home-page",

  components: {
    RegistrationForm,
  },
};
</script>

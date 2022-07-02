<template>
  <div>
    <!-- <h1>Formulario de: {{ nome }}</h1> -->
    <!-- <Form /> -->
    <Info :email="email" />
  </div>
</template>

<script>
import Info from "./Info.vue";
import Form from "./Form.vue";

export default {
  name: "Pessoa",
  components: {
    Info,
    Form,
  },
  data() {
    return {
      nome: "MJR",
      email: "",
    };
  },
  methods: {},
};
</script>

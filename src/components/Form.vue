<template>
  <form action="" @submit="enviarFormulario($event)">
    <input v-model="name" placeholder="nome" />
    <input v-model="email" placeholder="email" />
    <Submit />
  </form>
</template>

<script>
import InputText from "./form/InputText.vue";
import Submit from "./form/Submit.vue";

export default {
  nome: "Form",
  components: {
    InputText,
    Submit,
  },
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log(`o nome é ${name}`);
      console.log(`o email é ${email}`);
    },
  },
};
</script>

<template>
  <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
  name: "LifeCycle",
  data() {
    return {
      nome: "Ainda não sei",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Junior";
    }, 3000);
  },

  mounted() {
    setTimeout(() => {
      this.nome = "Maicel Junior";
    }, 5000);
  },
};
</script>

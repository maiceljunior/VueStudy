<template>
  <div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <Reutilizar />

    <MultiplosEventos />
  </div>
</template>

<script>
import MultiplosEventos from "./MultiplosEventos.vue";
import Reutilizar from "./Reutilizar.vue";

export default {
  name: "PrimeiroComponente",
  components: {
    MultiplosEventos,
    Reutilizar,
  },
  data() {
    return {
      nome: "Maicel",
      profissao: "Desenvolvedor",
    };
  },
};
</script>

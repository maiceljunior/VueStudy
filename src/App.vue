<template>
  <div>
    <!-- <Header /> -->
    <!-- <PrimeiroComponente /> -->
    <!-- <p>O dado de app é: {{ testando }}</p> -->
    <!-- <LifeCycle /> -->
    <!-- <Info /> -->
    <Pessoa />
  </div>
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";
import Info from "./components/Info.vue";
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Info,
    Header,
  },
  data() {
    return {
      testando: "Teste",
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #333;
  color: #fff;
}

a {
  color: red;
}
</style>

<template>
  <div>
    <p>{{ email }}</p>
    <!-- <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>não estou trabalhando</p>
    <p>Utilizo as seguintes tecnologias:</p>

    <ul>
      <li v-for="(filme, index) in filme_teste" v-bind:key="index">
        {{ filme }}
      </li>
    </ul>

    <p>Utilizo as tec para front end</p> -->

    <!-- <ul> -->
    <!-- <li v-for="tecnology in frontEnd_tec" :key="tecnology.id"> -->
    <!-- {{ tecnology.languages }} -->
    <!-- </li> -->
    <!-- </ul> -->

    <!-- <div> -->
    <!-- <button @click="showEmail">Esconder</button> -->
    <!-- </div> -->
    <!-- <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p> -->

    <!-- <p> -->
    <!-- Para acessar meu portfolio -->
    <!-- <a v-bind:href="Picture" target="_blank">basta clicar aqui</a> -->
    <!-- </p> -->

    <Picture />
  </div>
</template>

<script>
import Picture from "./Picture.vue";

export default {
  nome: "Info",

  data() {
    return {
      esta_trabalhando: true,
      mostrar_email: true,
      Picture,
      filme_teste: ["aedsa", "dfgdfg", "sdaaaa"],
      frontEnd_tec: [
        { id: 1, languages: "PHP" },
        { id: 2, languages: "HTML" },
        { id: 3, languages: "CSS" },
      ],
    };
  },
  props: {
    email: String,
  },
  components: {
    Picture,
  },
  methods: {
    showEmail() {
      this.mostrar_email = !this.mostrar_email;
    },
  },
};
</script>

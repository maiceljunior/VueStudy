<template>
  <img :src="avatar" :alt="descricao" />
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/public/avatar.png",
      descricao: "Maicel Junior",
    };
  },
};
</script>

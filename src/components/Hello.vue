<template>
  <div class="hello">
    <h1>Bem Vindo {{ nome }}!</h1>
  </div>
</template>

<script>
export default {
  name: "Hello",
  props: {
    nome: String,
  },
};
</script>

<style scoped>
h1 {
  font-size: 40px;
  color: #00000b;
}
</style>

<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <br />
    <input v-model="nameUser" class="input" placeholder="Digite seu nome" />
    <Hello :nome="nameUser" />
    <HelloWorld msg="Esse é o mundo do Vue.js" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Hello from "./components/Hello.vue";

export default {
  name: "App",
  data() {
    return {
      nameUser: "",
    };
  },
  components: {
    HelloWorld,
    Hello,
  },
  watch: {
    nameUser() {
      console.log(this.nameUser);
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

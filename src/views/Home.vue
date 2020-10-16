<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <Main msg="Welcome to Your Vue.js + TypeScript App" />
    <Nav />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Main from "@/components/Main.vue"; // @ is an alias to /src
import Nav from "@/components/Nav.vue";

@Options({
  components: {
    Main,
    Nav
  },
})
export default class Home extends Vue {}
</script>

<style scoped>
#nav {
  position: fixed;
}
</style>

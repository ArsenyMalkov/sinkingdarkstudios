<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/wiki">Wiki</router-link> |
    <router-link to="/about">About</router-link>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

export default class Main extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#nav {
  padding-top: 30px;
  padding-bottom: 30px;
  width: 100%;
  top: 0;
  left: 0;
  background-color: rgba(0, 0, 0, 0.87);
}

#nav a {
  font-weight: bold;
  color: #c47878;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #c62828;
}
</style>

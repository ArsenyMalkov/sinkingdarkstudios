<template>
  <Nav />
  <div class="wiki">
    <h1>This is an wiki page</h1>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Nav from "@/components/Nav.vue";

@Options({
  components: {
    Nav
  },
})
export default class Wiki extends Vue {}
</script>
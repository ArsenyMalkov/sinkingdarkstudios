<template>
  <Nav />
  <div class="about">
    <h1>This is an about page</h1>
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
export default class About extends Vue {}
</script>
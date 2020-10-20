<template>
  <Nav />
  <div class="wiki-container">
    <WikiItem name="Amulets" icon="amulets.svg" />
    <WikiItem name="Locations" icon="amulets.svg" />
    <WikiItem name="Characters" icon="amulets.svg" />
    <WikiItem name="Abilities" icon="amulets.svg" />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import Nav from "@/components/Nav.vue";
import WikiItem from "@/components/WikiItem.vue";

@Options({
  components: {
    Nav,
    WikiItem
  },
})
export default class Wiki extends Vue {}
</script>

<style scoped>
.wiki-container {
  display: grid;
  grid-template-columns: auto auto auto;
  justify-content: center;
  align-content: center;
  grid-row-gap: 50px;
  margin-top: 50px;
}
</style>
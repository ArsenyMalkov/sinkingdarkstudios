<template>
  <Nav />
  <div class="wiki-container">
    <WikiItem name="Amulets" icon="amulets.svg" bkgColor="rgb(141, 74, 207)" />
    <WikiItem name="Locations" icon="locations2.svg" bkgColor="rgb(79, 74, 207)" />
    <WikiItem name="Characters" icon="amulets.svg" bkgColor="rgb(207, 200, 74)" />
    <WikiItem name="Abilities" icon="amulets.svg" bkgColor="rgb(207, 74, 74)" />
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
@media only screen and (max-width: 600px) {
  .wiki-container {
    grid-template-columns: minmax(0, 1fr) minmax(0, 1fr) minmax(0, 1fr)
  }
}
</style>
<template>
  <Nav />
  <div class="wiki">
    <WikiItem />
    <!-- <ul>
      <li>Coffee</li>
      <li>Tea</li>
      <li>Milk</li>
    </ul> -->
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
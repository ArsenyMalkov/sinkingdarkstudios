<template>
  <div class="wiki-item">
    <img src="../assets/logo.svg" />
    <div class="content">
      <router-link to="/about">Name</router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    // msg: String
  }
})
export default class WikiItem extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wiki-item {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  border-radius: 5px;
  margin-left: 20px;
  margin-top: 20px;
  width: 10%;
}

.content {
  padding-top: 16px;
  padding-bottom: 16px;
}

.wiki-item:hover {
  box-shadow: 0 8px 8px 0 rgba(0,0,0,0.2);
}

img {
  width: 100%;
  border-radius: 5px 5px 0 0;
}

a {
  color: #bb0303;
}
</style>
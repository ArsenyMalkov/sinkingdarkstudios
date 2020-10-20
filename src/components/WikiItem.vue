<template>
  <div class="wiki-item">
    <img class="icon" :src="require(`@/assets/${icon}`)" />
    <div class="content">
      <router-link to="/about">{{name}}</router-link>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    icon: String,
    name: String
  }
})
export default class WikiItem extends Vue {
  icon!: string;
  name!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.icon {
  padding-top: 4px;
  width: 50%;
}

.wiki-item {
  width: 70%;
  margin: auto;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  border-radius: 5px;
  background-color: rgb(207, 74, 167);
}

.content {
  padding-top: 16px;
  padding-bottom: 16px;
  background-color: rgb(255, 255, 255);
}

.wiki-item:hover {
  box-shadow: 0 8px 8px 0 rgba(0,0,0,0.2);
}

img {
  border-radius: 5px 5px 0 0;
}

a {
  color: #bb0303;
}
</style>
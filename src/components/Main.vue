<template>
  <video id="bloodRainVideo" autoplay muted loop preload="auto">
    <source src="BloodRain.m4v" type=video/mp4>
    <source src="BloodRain.mkv" type="video/webm">
  Sorry, your browser doesn't support embedded videos, 
  but don't worry, you can <a href="BloodRain.mkv">download it</a>
  and watch it with your favorite video player!
  </video>
  <img id="logo" src="../assets/logo.svg" alt="Logo">
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    msg: String
  }
})
export default class Main extends Vue {
  msg!: string
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#bloodRainVideo {
  position: absolute;
  /* top: 79px; */
  bottom: 0;
  /* max-height: calc(100% - 79px); */
  height: 100%;
  width: 100%;
  object-fit: fill;
  display: block;
}
#logo {
  position: absolute;
  transform: translate(-50%, -50%);
  width: 40%;
  left: 50%;
  top: 50%;
}
</style>

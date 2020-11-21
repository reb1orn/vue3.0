<template>
  <div>
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Hello Vue 3.0 + Vite" />
    <Setup></Setup>
    <life></life>
    <reactive></reactive>
    <ref></ref>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Setup from './example/setup.vue'
import life from './example/life.vue'
import reactive from './example/reactive.vue'
import ref from './example/ref.vue'
export default {
  name: "App",
  components: {
    HelloWorld,
    Setup,
    life,
    reactive,
    ref
  },
};
</script>

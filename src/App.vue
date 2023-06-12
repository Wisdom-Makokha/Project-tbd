<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <a href="" target="_blank">
      <img src="./assets/58482ffecef1014c0b5e4a8f.png" class="logo" alt="RockStar" />
    </a>
  </div>
  <HelloWorld msg="hello world" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #b67c00);
}

</style>

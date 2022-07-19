<template>
  <div id="app">
    <HeaderMenu></HeaderMenu>
  </div>
</template>

<script>
import HeaderMenu from '@/components/HeaderMenu.vue'
export default {
  name: "App",
  components: {
    HeaderMenu,
  },
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}
#app {
  
}
</style>

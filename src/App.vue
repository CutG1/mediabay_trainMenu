<template>
  <div id="app">
    <HeaderMenu></HeaderMenu>
    <RegisForm/>
  </div>
</template>

<script>
import HeaderMenu from '@/components/HeaderMenu.vue'
import RegisForm from '@/components/RegistrationForm.vue'
export default {
  name: "App",
  components: {
    HeaderMenu,
    RegisForm
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

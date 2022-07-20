<template>
  <div id="app">
    <!-- <HeaderMenu></HeaderMenu> -->
    <component :is="comp" @changeComp="changeComp"></component>
  </div>
</template>

<script>
import HeaderMenu from '@/components/HeaderMenu.vue'
// import RegisForm from '@/components/RegistrationForm.vue'
import LogIn from '@/components/logIn.vue'  
import RegistrationSection from '@/components/RegistrationSection.vue'
export default {
  name: "App",
  components: {
    HeaderMenu,
    // RegisForm,
    LogIn,
    RegistrationSection
  },
  data() {
    return {
      comp: "HeaderMenu",
    }
  },
  methods: {
    changeComp(comp) {
      console.log(comp);
      this.comp = comp
    }
  }
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: sans-serif;
}
button{
  cursor: pointer;
}
#app {
  
}
</style>

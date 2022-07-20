<template>
  <div>
    <RegisForm @changeComp="changeComp" />
    <LogIn v-if="currentComp == 'LogIn'" />
    <RegistrationSection v-if="currentComp == 'RegistrationSection'" />
  </div>
</template>

<script>
import RegisForm from "@/components/RegistrationForm.vue";
import LogIn from "@/components/logIn.vue";
import RegistrationSection from "@/components/RegistrationSection.vue";
export default {
  components: {
    RegisForm,
    LogIn,
    RegistrationSection
  },
  data() {
    return {
      currentComp: "LogIn",
    };
  },
  methods: {
    changeComp(e){
        this.currentComp = e;
    }
  },
};
</script>

<style>
</style>
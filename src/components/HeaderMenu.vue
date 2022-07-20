<template>
  <div class="header">
    <div class="two_blocks">
      <div class="left">
        <img
          src="@/assets/whiteHam.jpg"
          alt="hamburger"
          width="50px"
          height="50px"
        />
        <img
          src="@/assets/iconLogo.png"
          alt="hamburger"
          width="50px"
          height="50px"
        />
        <h3>mediabay</h3>
      </div>
      <div class="rightContent">
        <button @click="$emit('changeComp', 'LogIn')">Войти</button>
      </div>
    </div>
  </div>
</template>

<script>
import LogIn from '@/components/logIn.vue'
export default {
  comments: {
    LogIn,
  }
};
</script>

<style scoped>
.header {
  width: 100%;
  height: 90px;
  padding: 20px 30px;
  background-color: rgb(44, 46, 54);
  color: white;
}
.left h3 {
  display: inline-block;
  vertical-align: top;
  margin-left: 10px;
  padding-top: 15px;
  text-transform: uppercase;
}
.left {
  cursor: pointer;
}
.two_blocks div {
  display: inline-block;
}
.rightContent {
  float: right;
  padding-top: 10px;
}
.rightContent button {
  background: transparent;
  padding: 10px 25px;
  border-radius: 20px;
  color: white;
  border: 1px solid white;
}
</style>
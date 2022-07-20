<template>
  <div class="backImg">
    <span>X</span>
    <div class="centerBlock">
      <img src="@/assets/mb_logo.svg" alt="" />
      <label>
        <h2 @click="$emit('changeComp', 'LogIn')">LogIn</h2>
        <h2 @click="$emit('changeComp', 'RegistrationSection')">
          Registration
        </h2>
      </label>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.backImg {
  background-image: url("https://mediabay.uz/static/media/content-blur-bg.28519694.jpg");
  width: 100%;
  height: 100vh;
}
span {
  position: absolute;
  top: 30px;
  right: 70px;
  font-size: 30px;
  color: white;
  cursor: pointer;
}
img {
  /* width: 250px; */
  height: 54px;
}
.centerBlock {
  display: flex;
  flex-direction: column;
  -webkit-box-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  align-items: center;
  padding-top: 10%;
}
label h2 {
  display: inline-block;
  font-size: 40px;
  font-weight: bold;
  color: white;
  border-bottom: 2px solid white;
  cursor: pointer;
}
label h2:first-child {
  margin-right: 10px;
}
/* label h2:last-child{
  opacity: 0.4;
} */
</style>
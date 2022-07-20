<template>
  <div class="backImg">
    <span @click="$emit('changeComp', 'HeaderMenu')">X</span>
    <div class="centerBlock">
      <img src="@/assets/mb_logo.svg" alt="" />
      <label>
        <h2 @click="$emit('changeComp', 'LogIn')">LogIn</h2>
        <h2 @click="$emit('changeComp', 'RegistrationSection')">
          Registration
        </h2>
      </label>
      <form>
        <h3>Login</h3>
        <input type="text" placeholder="email or login" />
        <h3>Email</h3>
        <input type="email" placeholder="email or login" />
        <h3>Password</h3>
        <input type="password" placeholder="..." />
        <button>Enter</button>
      </form>
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
.centerBlock {
  display: flex;
  flex-direction: column;
  -webkit-box-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  align-items: center;
  padding-top: 10%;
}
span {
  position: absolute;
  top: 30px;
  right: 70px;
  font-size: 30px;
  color: white;
  cursor: pointer;
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
img {
  height: 54px;
}
form {
  margin-top: 20px;
  text-align: center;
}
input {
  background: rgba(255, 255, 255, 0.1);
  padding: 15px 20px;
  font-size: 20px;
  outline: none;
  border: none;
  margin: 5px 0 35px 0;
  color: white;
}
input::placeholder {
  color: rgb(161, 161, 161);
}
h3 {
  font-size: 18px;
  color: aliceblue;
  text-align: left;
}
button {
  display: block;
  width: 100%;
  padding: 15px 0;
  font-size: 24px;
  background-color: #f90;
  border: none;
  outline: none;
  border-radius: 20px;
  color: white;
}
</style>
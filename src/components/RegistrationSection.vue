<template>
  <div>
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
</template>

<script>
export default {};
</script>

<style scoped>
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
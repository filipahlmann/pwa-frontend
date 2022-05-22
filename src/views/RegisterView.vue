<template>
  <div>
    <h1>Register</h1>
      <span> Test: {{ state.name }} </span>
      <br>
    <input type="text" placeholder="Name" v-model="state.name">
      <br>
      <span> Test: {{ state.email }} </span>
      <br>
    <input type="text" placeholder="Email" v-model="state.email">
      <br>
      <span> Test: {{ state.password }} </span>
      <br>
    <input type="text" placeholder="Password" v-model="state.password">
        <br>
    
  <!-- SwaggerRegister button -->

  <button @click="swaggerRegister()">Swagger Login</button>
  </div>
</template>

<script>
import todocrud from '../modules/todocrud'

  export default {
    setup() {

      const { state, swaggerRegister  } = todocrud()
      // REST API token added: swaggerLogin

      return { state, swaggerRegister }
      // REST API token added: swaggerLogin
    },
   
    
  }
</script>


<style>
input {
  width: 30%;
  box-sizing: border-box;
  border: 2px solid #2c3e50;
  border-radius: 4px;
  font-size: 16px;
  background-color: white;
  background-position: 10px 10px; 
  background-repeat: no-repeat;
  padding: 12px 20px 12px 40px;
  margin: 15px;
}

button {
  background-color: #2c3e50;
  color: white;
  border: none;
  padding: 20px;
    border-radius: 4px;

}
</style>


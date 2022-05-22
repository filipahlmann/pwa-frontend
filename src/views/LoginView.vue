<template>
  <div>
    <h1>Login</h1>

    <br>
    <input type="text" placeholder="Email" v-model="state.email">
        <br>
    <span> Test: {{ state.email }} </span>
    <br>
    <input type="text" placeholder="Password" v-model="state.password">
        <br>
    <span> Test: {{ state.password }} </span>
  <!-- SwaggerLogin button -->
      <br>

  <button @click="swaggerLogin()">Swagger Login</button>
  </div>
</template>

<script>
import todocrud from '../modules/todocrud'

  export default {
    setup() {

      const { state, swaggerLogin  } = todocrud()
      // REST API token added: swaggerLogin

      return { state, swaggerLogin }
      // REST API token added: swaggerLogin
    },
   
    
  }
</script>

<style lang="scss" scoped>

</style>
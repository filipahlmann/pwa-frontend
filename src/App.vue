
<template>
<div>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/todos">Todos</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/register">Register</router-link> |
    <router-link to="/login">Login</router-link> 

  </nav>
          <router-view/>
</div>
</template>



<style lang="scss">
body{
  margin: 0px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
    margin: 0px;

}
nav {
  background-color: #2c3e50;
;
  padding: 30px;
  a {
      padding: 30px;

    text-decoration: none;
    font-weight: bold;
    color: white;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
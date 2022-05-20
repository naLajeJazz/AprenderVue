<template>
  <div   id="app">
    <nav class="navbar navbar-light bg-dark mb-3">
      <div class="container-fluid">
      <a class="lk" href="">
<span class="navbar-brand mb-0 h1 text-light">Inicio</span>
</a>
</div>
    </nav>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
body{
  background-color: #2c3e50;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
  background-color: #2c3e50;
}
.lk{
  text-decoration: none;
}
</style>

<template>
  <div   id="app">
    <header>
      <nav class="navbar navbar-light bg-dark mb-2">
        <div class="container-fluid">
        <a class="lk" href="">
  <span class="navbar-brand mb-0 h1 text-light">Menu</span>
  </a>
  </div>
      </nav>
    </header>

<router-view />
<footer>
      <nav class=" bg-dark mt-2 static-bottom">
        <div class="container-fluid"> <a class="lk" href="">
  <span class="navbar-brand mb-0 h1 text-light">Desenvolvido por Rodrigo Melo</span>
  </a>
  </div>
      </nav>
    </footer>
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
footer{
  width: 100%;
}
.imag{
  width: 2em;
}
</style>

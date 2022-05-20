<template>
  <div class="hello">

    <div class="container text-dark card ">
  <div class="row align-items-start ">
    <div class="col">
      <img  src="../assets/logo.png">
    </div>
    <div class="col ">
      info
    </div>
  </div>
</div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 10,
      msgb: 10
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;

}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

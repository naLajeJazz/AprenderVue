<template>
  <div  class="hello"> <div class="container text-dark card ">
  <div class="row align-items-start ">
    <div class="col">
      <img width="150px" :src="img" alt="img" />
    </div>
    <div class="col  ">
     Classe: {{msg}}
    </div>
  </div>
</div>
    <div class="container text-dark card my-4 ">
  <div class="row align-items-start ">
    <div class="col">
      <img width="280px" :src="img2" alt="img" />
    </div>
    <div class="col  ">
     Classe: {{msg2}}
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
      img: 'https://i.imgur.com/ANhvnbE.gif',
      img2: 'https://i.pinimg.com/originals/91/05/3a/91053ac18b8b3368d29a1409ad6be5f1.gif',
      msg: 'Arcano',
      msg2: 'Bardo'
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

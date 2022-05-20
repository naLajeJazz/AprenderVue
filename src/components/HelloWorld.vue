<template>
  <div  class="hello"> <div class="container text-dark card mt-4 ">
  <div class="row align-items-start ">
    <div class="col">
      <img width="100%" :src="img" alt="img" />
    </div>
    <div class="col  ">

   <h3 class="text-start"> Xp:{{xp}}</h3>
   <h3 class="text-start">Classe: {{classe}}</h3>
   <h4 v-if="msgCond" class="text-start text-info">Disponivel</h4>
   <h4 v-else-if="!msgCond" class="text-start text-danger">Indiponivel</h4>
<div>
  <h5 class="text-dark">Items</h5>
  <ul class="list-group list-group-flush my-3 ">
    <li class="text-dark list-group-item align-items-center" v-for="atr in atributos">
    {{atr}}
    </li>
</ul>

</div>
    </div>
  </div>
</div>
<button class="btn btn-dark my-3 " @click="xp--" >Próximo</button>

    </div>
</template>

<script>
/* eslint-disable no-new */
let bl= true
let img=['https://i.imgur.com/ANhvnbE.gif',
'https://i.pinimg.com/originals/91/05/3a/91053ac18b8b3368d29a1409ad6be5f1.gif']
let classe=['Arcano','Bardo']

export default {
  name: 'HelloWorld',
  data () {
    return {
      img: img[0],
      classe: classe[0],
      msgCond: bl,
      xp: 10,
      atributos: ['Cajado','Capa Mágica','Adaga']
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

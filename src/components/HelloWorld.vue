<template>
  <div  class="hello"> <div class="container text-dark card mt-4 ">
  <div class="row align-items-start ">
    <div class="col">
      <img width="100%" :src="img" alt="img" />
    </div>
    <div class="col  ">

   <h3 v-if="xp<10" class="text-start"> Xp:{{xp}}</h3>
   <h3 class="text-start">Classe: {{classe}}</h3>
   <h5 v-if="msgCond" class="text-start text-info">Disponivel</h5>
   <h5 v-else-if="!msgCond" class="text-start text-danger">Indiponivel</h5>
<div>
  <h5 class="text-dark">Items</h5>
  <ul class="list-group list-group-flush my-3 ">
    <li class="text-dark list-group-item align-items-center" v-for="atr in atributos" :key="atr.id">
    {{atr}}
    </li>
</ul>

</div>
    </div>
  </div>
</div>
<button class="btn btn-dark my-3 " @click="voltar()" >Voltar</button>
<button class="btn btn-dark my-3 " @click="proximo()" >Próximo</button>
</div>

</template>

<script>

let img = ['https://i.imgur.com/ANhvnbE.gif', 'https://i.pinimg.com/originals/91/05/3a/91053ac18b8b3368d29a1409ad6be5f1.gif']
let classe = ['Arcano', 'Bardo']
let atrib = [['Cajado', 'Capa Mágica', 'Adaga'], ['Bandolin', 'Botas', 'Colar Mágico']]

export default {
  name: 'HelloWorld',
  data () {
    return {
      img: img[0],
      classe: classe[0],
      msgCond: false,
      xp: 0,
      atributos: atrib[0],
      proximo: function () { this.atributos = atrib[1]; this.img = img[1]; this.classe = classe[1] },
      voltar: function () { this.atributos = atrib[0]; this.img = img[0]; this.classe = classe[0] }
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
img{
  border: 1px solid #2c3e50;
  border-radius: 30px;
  margin-top: 20px;
  margin-bottom: 20px;
}
</style>

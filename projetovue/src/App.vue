<template>
  <div id="app">
    <!-- <h1>Olá</h1> -->
    <!-- props -->
    <!-- reatividade com props -->
    <input type="text" v-model="lotacao">
    <Cliente :nome="lotacao" idade="22" email="gabriellouredo.ti"/>
    <Cliente nome="Gabriel Ferreira" idade="22" email="gabriellouredo.ti"/>
    <input type="text" v-model="dadosFunc.nome">
    <Cliente :dados="dadosFunc"/>
   
  </div>
</template>

<script>

import Cliente from './components/Cliente';

export default {
  name: 'App',
  data(){
    return{
      lotacao: "SEMAD - Departamento de Sistemas",
      // variavel de objeto
      dadosFunc: {
        nome: "Gabriel Louredo",
        telefone: "99458679"
      }
    
    }
  },
  components:{
    Cliente,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color:black;
  margin-top: 60px;
}
</style>



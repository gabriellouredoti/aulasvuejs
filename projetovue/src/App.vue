<template>
  <div id="app">
    <h1>Olá</h1>
    <cliente/>
    <produtos/>

    
  </div>
</template>

<script>

import Cliente from './components/Cliente';
import Produtos from './components/Produtos';

export default {
  name: 'App',
  components:{
    Cliente,
    Produtos
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>



<template>

  <TheHeader></TheHeader>

</template>

<script>

import TheHeader from './components/TheHeader.vue';


export default {
  name: 'App',
  components: {
    TheHeader
  },
  data(){
    return{
      showHeader: true,
      name: 'xampson',
      acessLevel: 'admin',
    }
  }
}

</script>

<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

</style>

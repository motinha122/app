<template>
  <div class="card"></div>
  <PropsAlert :variant='variant'>
    {{text}}
  </PropsAlert>
</template>

<script>
import PropsAlert from '@/components/PropsAlert.vue';

export default {
  name: 'App',
  components: {
    PropsAlert
  },
  data() {
    return {
      variant:'success',
      text:'Formulário enviado com sucesso!'
    }
  }
}

</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Jost&display=swap');

#app {
  font-family: 'Jost', Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

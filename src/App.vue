<template>
  <div class="card"></div>
  <EmitAlert :variant='variant' @close="onClose()" v-if="showAlert" >
    {{text}}
  </EmitAlert>
</template>

<script>
import EmitAlert from '@/components/EmitAlert.vue';

export default {
  name: 'App',
  components: {
    EmitAlert
  },
  data() {
    return {
      showAlert:true,
      variant:'success',
      text:'Formulário enviado com sucesso!'
    }
  },
  methods:{
    onClose(){
      this.showAlert = false;
      console.log('close clickado');
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

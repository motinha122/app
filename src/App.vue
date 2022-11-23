<template>

  <VonEvent></VonEvent>

</template>

<script>
import VonEvent from './components/VonEvent.vue';


export default {
  name: 'App',
  components: {
    VonEvent
  },
  data() {
    return {

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

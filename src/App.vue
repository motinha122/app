<template>

  <CompProp></CompProp>

</template>

<script>
import CompProp from './components/CompProp.vue';


export default {
  name: 'App',
  components: {
    CompProp
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

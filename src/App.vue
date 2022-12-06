<template>
  <TheHeader v-if="showHeader">
    <template v-slot:title>
      Title
    </template>
    <template v-slot:description>
      Description
    </template>
  </TheHeader>
  <LifeCycle></LifeCycle>
  <button @click="showHeader = !showHeader">Show Header</button>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue';
import TheHeader from './components/TheHeader.vue';

export default {
  name: 'App',
  components: {
    LifeCycle,
    TheHeader
},
  data() {
    return {
      showHeader: true,
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

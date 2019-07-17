<template>
  <div id="app">

      <Header1 class="header-map"></Header1>
<!--        <Box/>-->
    <SensorChoices/>
  </div>
</template>

<script>
  //import Hello from './components/Hello.vue';
  import Header1 from './components/Header1.vue';
  // import Box from './components/Dialog.vue';
  import Button from './components/Button.vue';
  import Map from './components/Map.vue';
  import Popup from './components/Popup.vue';
  //import SensorChoices from './components/SensorChoices.vue';
  import store from 'store';
  //import Box from "components/Box";

  export default {
    name: 'App',
    components: {
      Header1
        // Box
      //SensorChoices
    }
  }

  //store.commit('increment');
  //console.log(store.getters.evenOrOdd);
  //store.commit('increment');
  //console.log(store.getters.evenOrOdd);
  //console.log(store.state.count);
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 0;
  }

  .header-map{
      margin-bottom: 300px;

  }


</style>
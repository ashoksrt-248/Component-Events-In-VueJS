<template>
  <div id="app">
    <h1> Component Events</h1>
    <button @click="showPopup = true">Show Popup</button>
    <Popup  v-show="showPopup" @close="showPopup = false"/>
  </div>
</template>

<script>
import Popup from './components/Popup.vue';
export default {
  name: 'App',
  components:{
    Popup,
  },
  data(){
    return{
      showPopup:false
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
button{background-color:teal;width: 140px;height: 40px;border: 2px solid tomato;border-radius: 5px;}
</style>

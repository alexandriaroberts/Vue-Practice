<template>
  <div id="app">
    <flower-game id="game" :speed="10" :duration="60" :width="600" :height="550"/>
  </div>
</template>

<script>
import FlowerGame from "./components/FlowerGame.vue";
export default {
  name: "app",
  components: {
    FlowerGame
  }
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Amatic+SC');
body {
  height: 100%;
  background: rgb(43, 205, 179);
  /* background: linear-gradient(to center, rgb(43, 205, 179), #f7f8f8); */
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

#game {
  position: relative;
  overflow: hidden;
  margin: 0 auto;
  height: 100%;
  background: #283c86;
  /* background: -webkit-linear-gradient(to left, #45a247, #283c86);
  background: linear-gradient(to left, #45a247, #283c86); */
   box-shadow: 2px 2px 5px 0px rgba(0,1,25,1);
   border-radius: 5px;
}
</style>

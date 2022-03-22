<template>
  <div id="app">
   <Header/>
  </div>
</template>

<script>
import Header from './components/MainHeader.vue'

export default {
  name: 'App',
  components: {
    Header,
    
  }
}
</script>

<style lang="scss">
:root {
  --main-green: #85b680 ;
  --over-green: #79b27b ;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  min-height: 100vh;
  min-width: 1920px;
  font-size: 1.5 rem ;
}
</style>

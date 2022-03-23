<template>
  <div id="app">
   <Header/>
   <Footer/>
  </div>
</template>

<script>
import Header from './components/MainHeader.vue'
import Footer from './components/MainFooter.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    
  }
}
</script>

<style lang="scss">
:root {
  --main-green: #85b680 ;
  --over-green: #79b27b ;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
ul,ol{
  list-style: none;
  a{
    color: currentColor;
  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  min-height: 100vh;
  min-width: 1920px;
  font-size: 1.5 rem ;
}
.container-fluid{
  min-width: 1920px
}
.container {
  width: 1180px;
  margin: 0 auto;
  display: flex;
}
.flex{
  display: flex;
}
</style>

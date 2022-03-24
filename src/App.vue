<template>
  <div id="app">
    <Header />
    <Form />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/MainHeader.vue";
import Footer from "./components/MainFooter.vue";
import Form from "./components/MainForm.vue";

export default {
  name: "App",
  components: {
    Header,
    Form,
    Footer,
  },
};
</script>

<style lang="scss">
:root {

  --text-xs: #7f9ea8;
  --main-green: #85b680;
  --over-green: #79b27b;
  --lightGrey: #e5e8eb;
  --darkGrey: #484848;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
ul,
ol {
  list-style: none;
  a {
    color: currentColor;
  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  min-height: 100vh;
  min-width: 1920px;
  font-size: 1.5 rem;
}
.nav-bar,
.green_button {
  font-size: 16px;
  font-weight: bold;
  text-transform: uppercase;
}
.green_button {
  color: white;
  background-color: var(--main-green);
  padding: 10px 20px;
  border-radius: 29px;
  border: 2px solid transparent;
  text-align: center;
  min-width: 145px;
  height: 46px;
  display: block;
  &:hover {
    background-color: var(--over-green);
  }
}
.container-fluid {
  min-width: 1920px;
}
.container {
  width: 1180px;
  margin: 0 auto;
  display: flex;
}
.container-half {
  width: 41%;
  margin-right: 5%;
}
.flex {
  display: flex;
}
#logo {
  img {
    width: 260px;
  }
}
</style>

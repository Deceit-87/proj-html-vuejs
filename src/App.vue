<template>
  <div id="app">
    <Header />
    <Form />
    <Courses />
    <Instructor />
    <Testimonials />
    <LatestNews />
    <NewsLetter />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/MainHeader.vue";
import Footer from "./components/MainFooter.vue";
import Form from "./components/MainForm.vue";
import Courses from "./components/MainCourse.vue";
import Instructor from "./components/MainInstructor.vue";
import Testimonials from "./components/MainTestimonials.vue";
import LatestNews from "./components/MainNews.vue";
import NewsLetter from "./components/MainLetter.vue";

export default {
  name: "App",
  components: {
    Header,
    Form,
    Courses,
    Instructor,
    Testimonials,
    LatestNews,
    NewsLetter,
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
  font-family: "Montserrat", sans-serif;
  font-family: "Mulish", sans-serif;
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
.sec_button {
  border-radius: 25px;
  font-size: 12px;
  font-weight: 700;
  padding: 8px 18px;
  border: 3px solid var(--text-xs);
  transition: all 0.3s ease;
  text-transform: uppercase;
  background-color: #fff;
  color: var(--text-xs);
  transition: all 0.5s;
  &:hover {
    border: 3px solid var(--over-green);
    color: var(--over-green);
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
h3 {
  font-size: 42px;
  font-weight: 700;
}
</style>

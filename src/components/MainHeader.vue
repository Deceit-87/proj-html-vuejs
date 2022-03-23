<template>
  <header id="header">
    <div class="container-fluid">
      <div class="container-fluid contact-header">
        <div class="container">
          <p>We have a 95% Successful Pass Rate!</p>
          <p>Give us a call to book your tuition! 1-800-555-555</p>
        </div>
      </div>
      <div class="container-fluid nav-bar">
        <div class="container">
          <figure id="header_logo">
            <img src="../assets/img/avada-drivers-logo-2x.png" alt="" />
          </figure>
          <ul class="nav-ul">
            <li v-for="(link, i) in links" :key="i">
              <a :href="link.page_link"> {{ link.page_index }}</a
              ><span class="update" v-if="link.news === true">new</span>
            </li>
          </ul>
          <button class="header_button">book now</button>
        </div>
      </div>
    </div>
    <div class="container jumbo">
      <h1>Drive with Avada</h1>
      <p>We offer the finest driving tuition money can buy</p>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          page_index: "home",
          page_link: "https://www.google.it/",
          news: false,
        },
        {
          page_index: "about",
          page_link: "https://www.google.it/",
          news: false,
        },
        {
          page_index: "price",
          page_link: "https://www.google.it/",
          news: false,
        },
        {
          page_index: "courses",
          page_link: "https://www.google.it/",
          news: true,
        },
        {
          page_index: "location",
          page_link: "https://www.google.it/",
          news: false,
        },
        {
          page_index: "blog",
          page_link: "https://www.google.it/",
          news: false,
        },
      ],
    };
  },
};
</script>


<style scoped lang="scss">
#header {
  display: flex;
  flex-direction: column;
  background-image: url("../assets/img/homepage-hero-background.jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 782px;
  .jumbo {
    display: flex;
    color: white;
    flex-direction: column;
    justify-content: center;
    flex-grow: 1;
    h1 {
      font-size: 63px;
    }
    p {
      font-size: 27px;
    }
  }
  .contact-header {
    background-color: #484848;
    height: 30px;
    .container {
      color: #7f9ea8;
      display: flex;
      justify-content: space-between;
      font-size: 12px;
    }
  }
  .nav-bar,
  .header_button {
    font-size: 16px;
    font-weight: bold;
    text-transform: uppercase;
  }
  .nav-bar {
    display: flex;
    height: 120px;
    background-color: #0b0b0b52;
    color: white;
    .container {
      display: flex;
      align-items: center;
      justify-content: space-between;
      #header_logo {
        padding: 20px;

        img {
          width: 260px;
        }
      }

      ul {
        gap: 50px;
        display: flex;
        li {
          position: relative;
        }
        li a:hover{
          color: var(--over-green);
           transition: all 0.5s;

        }
        li a:hover::after {
          content: "";
          opacity: 1;
          bottom: -10px;
          width: 100%;
          transition: all 0.5s;
        }
        li a:after {
          content: "";
          display: block;
          position: absolute;
          left: 50%;
          opacity: 0;
          transform: translate(-50%, 0);
          bottom: -10px;
          width: 0px;
          height: 2px;
          background-color: var(--over-green);
        }
        .update {
          background-color: var(--main-green);
          margin-left: 7px;
          border-radius: 5px;
          padding: 1px 4px;
        }
      }
    }

    a {
      text-decoration: none;
      
    }
    .header_button {
      color: currentColor;
      background-color: var(--main-green);
      padding: 10px 20px;
      border-radius: 29px;
      border: 2px solid transparent;
      text-align: center;
      width: 145px;
      height: 46px;
      display: block;
    }
  }
}
</style>

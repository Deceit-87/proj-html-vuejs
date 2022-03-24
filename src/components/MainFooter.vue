<template>
  <footer id="footer" class="container-fluid">
    <div class="container">
      <div class="footer-card">
        <figure id="logo">
          <img
            src="../assets/img/avada-ad-drivers-logo-2x.png"
            alt="avada logo"
          />
        </figure>
        <p>
          Avada Driving School is the right choice for experienced drivers
          looking for a refresher course, or the brand new driver wanting to
          pass first time.
        </p>
      </div>
      <div class="footer-card">
        <h3 class="">contats details</h3>
        <ul class="">
          <li class="flex">
            <i class="fas fa-home"></i>
            12345 North Main Street, New York, NY 555555
          </li>
          <li>
            <i class="fas fa-phone"></i>
            1.800.555.6789
          </li>
          <li>
            <i class="fas fa-envelope"></i>
            info@your-domain.com
          </li>
          <li>
            <i class="fas fa-link"></i>
            Theme-Fusion.com
          </li>
        </ul>
      </div>
      <div class="footer-card course">
        <h3 class="ad-h3">courses</h3>
        <ul>
          <li v-for="link in footerLinks" :key="link">
            <i class="far fa-arrow-alt-circle-right"></i>
            <a :href="link.url_link">{{ link.name_link }}</a>
          </li>
        </ul>
      </div>
      <div class="footer-card offert-grid">
        <figure class="grid">
          <img src="../assets/img/footer-grid.png" alt="" />
        </figure>

        <button class="green_button">book now</button>
      </div>
    </div>
    <div class="container-fluid credits">
      <div class="container">
        <div>
          <p>
            © Copyright 2012 - 2020 | Avada Theme by
            <a href="#">ThemeFusion</a>
            | All Rights Reserved | Powered by
            <a href="#">WordPress</a>
          </p>
        </div>
        <div>
          <div class="social-link">
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      footerLinks: [
        { name_link: "Pass Plus", url_link: "#" },
        { name_link: "Intensive Course", url_link: "#" },
        { name_link: "Automatic", url_link: "#" },
        { name_link: "Instructor Training", url_link: "#" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#footer {
  font-size: 18px;
  color: var(--text-xs);
  height: 591px;
  background-image: url("../assets/img/footer-background-color.jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  i{
      padding-right: 15px;
  }
  .credits{
      background-color: black;
      position: absolute;
      height: 150px;
      width: 100%;
      position: absolute;
bottom: -100px;
.container{
    font-size: 12px;
    display: flex;
    justify-content: space-between;
}
a{
    color: var(--main-green);
    text-decoration: none;
}
i{
    color: #ffffff;
}
      
  }
  .container {
    padding-top: 65px;
    .footer-card.offert-grid {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .footer-card.course{
        color:var(--main-green)
    }
    .footer-card {
      width: 23%;
      height: 320px;
      margin: 1%;
      .grid {
        padding-bottom: 24px;
        img {
          width: 100%;
          height: 245px;
        }
      }
      ul li {
        padding-bottom: 12px;
        padding-right: 45px;
        a {
          text-decoration: none;
        }
      }
      h3,
      .button_green {
        text-transform: uppercase;
      }
      h3 {
        padding-bottom: 30px;
        color: white;
        font-weight: 700;
      }
      #logo {
        padding-bottom: 15px;
      }
    }
  }
}
</style>


<template>
  <footer id="footer" class="container-fluid">
    <div class="container">
      <div class="footer-card">
        <figure id="logo">
          <img src="../assets/img/avada-drivers-logo-2x.png" alt="avada logo" />
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
            <span class="fas fa-home"></span>
            12345 North Main Street, New York, NY 555555
          </li>
          <li>
            <span class="fas fa-phone"></span>
            1.800.555.6789
          </li>
          <li>
            <span class="fas fa-envelope"></span>
            info@your-domain.com
          </li>
          <li>
            <span class="fas fa-link"></span>
            Theme-Fusion.com
          </li>
        </ul>
      </div>
      <div class="footer-card">
        <h3>courses</h3>
        <ul>
          <li v-for="link in footerLinks" :key="link" class="courses">
            <span class="far fa-arrow-alt-circle-right icon-green"></span>
            <a :href="link.url_link">{{ link.name_link }}</a>
          </li>
        </ul>
      </div>
      <div class="footer-card">
        
          <img src="../assets/img/labels.png" alt="" />
        
        <button class="green_button">book now</button>
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
    color:var(--text-xs);
  height: 591px;
  background-image: url("../assets/img/footer-background-color.jpg");
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  .container {
    padding-top: 65px;
    .footer-card {
      width: 23%;
      height: 320px;
      margin: 1%;
      border: 1px solid red;
      ul li{
          padding-right:75px;
          a{
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


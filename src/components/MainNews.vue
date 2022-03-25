<template>
  <section id="news" class="container-fluid">
    <div class="container last-news_wrapper">
      <h2>Latest News</h2>
      <div class="container">
        <div class="container-half">
          <div class="chose-car">
            <a href="#"
              ><img src="../assets/img/blog-choosecar.jpg" alt="blog-choosecar"
            /></a>
          </div>
          <a href="#">What Car to Start With?</a>
          <p>
            February 7th, 2019 | <a href="#">0 Comments</a>
          </p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
        </div>
        <div class="container-half">
          <div class="chose-car">
            <a href="#"
              ><img src="../assets/img/blogpost-10and2-700x441.jpg" alt="blog-choosecar"
            /></a>
          </div>
          <a href="#">What Car to Start With?</a>
          <p>
            February 7th, 2019 | <a href="#">0 Comments</a>
          </p>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
        </div>
      </div>
      <button class="green_button">More from the blog</button>

      <div class="container news-bottom"></div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
#news {
  min-height: 904px;
  background-image: url("../assets/img/latestnews-background.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  .last-news_wrapper {
    flex-direction: column;
    align-items: center;
    background: #fff;
    border-top: 6px solid var(--deepBlue);
    border-radius: 10px;
    height: 759px;
    position: relative;
    top: -40px;
    box-shadow: 0px 25px 20px 0px rgba(155, 155, 155, 0.71);
    h2 {
      font-size: 40px;
      font-weight: 800;
      color: var(--darkGrey);
      padding-top: 80px;
      padding-bottom: 62px;
    }
    .container{
        justify-content: center;
padding-bottom: 72px;
gap: 33px;
        .container-half{
              display: flex;
  flex-direction: column;
  align-items: center;
  width: 44%;
  margin: 0;
  .chose-car img{
      width: 513px;
      height: 322px;
  }
}

        }
    }
  }

</style>
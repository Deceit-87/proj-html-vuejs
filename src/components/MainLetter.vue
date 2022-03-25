<template>
  <section id="news_letter">
    <div class="container-md">
      <div class="form-wrapper">
        <h3>Sign up to our Newsletter</h3>
        <form>
          <input type="email" name="email" />
          <button type="submit" class="green_button">Subscribe</button>
        </form>
        <p>
          (We do not share your data with anybody, and only use it for its
          intended purpose)
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss">
#news_letter {
  min-height: 406px;
  background-image: url("../assets/img/newsletter_background.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  .form-wrapper {
    text-align: center;
    padding-top: 60px;
    padding-bottom: 74px;
    width: 100%;
    h3 {
      font-size: 30px;
      color: var(--darkGrey);
      padding-bottom: 46px;
      font-weight: 700;
    }
    input {
      width: 100%;
      height: 54px;
      border-radius: 1px;
      margin-bottom: 33px;
      outline: none;
      border: 1px solid var(--lightGrey);
    }
    button {
      width: 100%;
      margin-bottom: 40px;
    }
    p {
      color: var(--text-xs);
      font-size: 14px;
    }
  }
}
</style>
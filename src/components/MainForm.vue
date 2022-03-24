<template>
  <section class="form-container container-fluid">
    <div class="container">
      <div class="container-half">
        <h2>Get Behind The Wheel</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices
          auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices
          auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.
          Fusce et ultrices libero, at suscipit lacus. Sed vitae fringilla nibh.
          Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in
          vehicula semper. Fusce et ultrices libero, at suscipit lacus. Sed
          vitae fringilla nibh.
        </p>
      </div>
      <div class="container-half">
        <div class="form-wrapper">
          <h3>First Lesson Free!</h3>
          <p>
            When you make a block booking with us your first lesson is included
            free.
          </p>
          <form action="">
            <input
              type="text"
              name="name"
              placeholder="Your Name"
              minlength="3"
            />
            <input
              type="email"
              name="email"
              placeholder="Email"
              minlength="3"
            />
            <input
              type="text"
              name="phone"
              placeholder="Telephone"
              minlength="3"
            />
            <input
              type="text"
              name="location"
              placeholder="Location"
              minlength="3"
            />
            <button type="submit" class="green_button" name="button">
              request a callback
            </button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>


<style lang="scss" scoped>
.form-container {
  position: relative;
  min-height: 705px;
  .container {
    padding-top: 100px;
    .form-wrapper {
      min-height: 659px;
      display: flex;
      flex-direction: column;
      align-items: center;
      box-shadow: 0px 25px 20px 0px rgba(211, 211, 211, 0.486);
      position: absolute;
      top: -5%;
      background-color: #fff;
      border-radius: 10px;
      form {
        display: flex;
        flex-direction: column;
      }
    }
  }
}
</style>>


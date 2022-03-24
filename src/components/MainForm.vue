<template>
  <section class="form-container container-fluid">
    <div class="container">
      <div class="container-half">
        <div class="form-info">
          <h3>Get Behind The Wheel</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc
            ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula
            semper.
          </p>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc
            ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula
            semper. Fusce et ultrices libero, at suscipit lacus. Sed vitae
            fringilla nibh. Nunc ultrices auctor sapien id cursus. Aliquam
            maximus turpis in vehicula semper. Fusce et ultrices libero, at
            suscipit lacus. Sed vitae fringilla nibh.
          </p>
        </div>
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
          </form>
          <button type="submit" class="green_button" name="button">
            request a callback
          </button>
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
  min-height: 673px;
  .container {
    padding-top: 85px;

    .form-info {
      h3 {
        font-size: 42px;
        font-weight: 800;
        padding: 0px 0 34px 0;
        color: var(--darkGrey);
      }

      p {
        font-size: 23px;
        font-weight: 700;
        line-height: 35px;
        padding: 0 0 30px 0;
        letter-spacing: -2px;
        color: var(--text-xs);
      }
      p:last-child {
        line-height: 32px;
        letter-spacing: -1px;
        font-size: 16px;
        color: var(--text-xs);
        width: 99%;
      }
    }
    .form-wrapper {
      padding: 40px;

      min-height: 634px;
      display: flex;
      flex-direction: column;
      align-items: center;
      box-shadow: 0px 25px 20px 0px rgba(211, 211, 211, 0.486);
      position: absolute;
      top: -6%;
      background-color: #fff;
      border-radius: 10px;
      p {
        width: 92%;
        text-align: center;
        line-height: 30px;
        padding-bottom: 36px;
        color: var(--text-xs);
        font-weight: 800;
      }
      h3 {
        font-size: 30px;
        font-weight: 801;
        color: var(--main-green);
        padding-bottom: 40px;
      }
      form {
        width: 100%;

        display: flex;
        flex-direction: column;

        input {
          margin-bottom: 28px;
          height: 50px;
          border-radius: 5px;
          box-shadow: none;
          border: 1px solid lightgray;
          padding-left: 12px;
          background-color: var(--lightGrey);
          &::placeholder {
            font-size: 12px;
            color: rgba(71, 71, 71, 0.8);
          }
          &:focus {
            outline: none;
            box-shadow: none;
            border-color: rgba(71, 71, 71, 0.4);
          }
        }
      }
    }
  }
}
</style>


<template>
  <section id="courses">
    <div class="header-courses container-fluid">
      <div class="container">
        <div class="courses-title">
          <h3>Start Learning to Drive Today</h3>
          <h2>Give us a call to schedule your first driving lesson</h2>
        </div>
        <div class="courses-contact">
          <i class="fusion-li-icon fa-phone fas"></i>
          <span>1-800-555-555</span>
        </div>
      </div>
    </div>

    <!-- COURSES  -->

    <div class="container-fluid courses">
      <div class="container">
        <div class="courses-info">
          <img class="corner-new" src="../assets/img/new-corner.jpg" alt="" />
          <h2>Courses</h2>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc
            ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula
            semper.
          </p>
          <button class="green_button">Course information</button>
        </div>
        <div class="courses_learn-more">
          <div class="learn-more_card">
            <img src="../assets/img/courses-passplus.jpg" alt="" />
            <h4>Pass Plus</h4>
            <button class="sec_button">Learn More</button>
          </div>
          <div class="learn-more_card">
            <img src="../assets/img/course-intensive.jpg" alt="" />
            <h4>Intensive Course</h4>
            <button class="sec_button">Learn More</button>
          </div>
          <div class="learn-more_card">
            <img src="../assets/img/courses-instructor.jpg" alt="" />
            <h4>Instructors</h4>
            <button class="sec_button">Learn More</button>
          </div>
        </div>
      </div>
    </div>

    <!-- RATE -->


    <div class="rate-container container-fluid">
      <div class="container">
        <div class="rate-card">
          <div class="circular">
            <div class="inner"></div>
            <div  class="number"><span> 95% </span></div>
            <div class="circle95">
              <div class="bar left95">
                <div class="progress"></div>
              </div>
              <div class="bar right95">
                <div class="progress"></div>
              </div>
            </div>
          </div>
          <p>PASS RATE</p>
        </div>
        <div class="rate-card">
          <div class="circular">
            <div class="inner"></div>
            <div  class="number"><span> 100% </span></div>
            <div class="circle100">
              <div class="bar left100">
                <div class="progress"></div>
              </div>
              <div class="bar right100">
                <div class="progress"></div>
              </div>
            </div>
          </div>
          <p>REFERRAL RATE</p>
        </div>
        <div class="rate-card">
          <div class="circular">
            <div class="inner"></div>
            <div  class="number"><span> 0% </span></div>
            <div class="circle">
              <div class="bar left">
                <div class="progress"></div>
              </div>
              <div class="bar right">
                <div class="progress"></div>
              </div>
            </div>
          </div>
          <p>ACCIDENT RATE</p>
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

<style lang="scss">
.container-fluid.courses {
  background-image: url(http://localhost:8081/img/promise-background.0e5d3981.jpg);
  background-size: cover;
  background-position: bottom;
  background-repeat: no-repeat;
  min-height: 520px;
}
.header-courses {
  display: flex;
  align-items: center;

  background: url("../assets/img/horizontal-cta-background.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top;
  min-height: 269px;
  .courses-title {
    flex-grow: 1;
  }
  .courses-title {
    color: #fff;
    flex-direction: column;
    justify-content: center;
    h3 {
      margin-top: -12px;
      padding-bottom: 5px;
    }
  }
  .courses-contact {
    display: flex;
    align-items: center;
    i {
      color: #fff;
      margin-right: 37px;
      font-size: 30px;
    }
    span {
      font-size: 33px;
      color: #fff;
      font-weight: 700;
      padding-right: 15px;
    }
  }
}
.courses-info {
  position: relative;
  box-shadow: 0px 25px 20px 0px rgba(155, 155, 155, 0.71);
  padding: 50px 30px;
  margin: 0 10px;
  border-radius: 10px;
  background-color: #fff;
  position: relative;
  bottom: 110px;
  overflow: hidden;
  top: -29px;
  margin-right: 45px;
  text-align: center;
  line-height: 34px;
  display: flex;
  flex-direction: column;
  align-items: center;
  .corner-new {
    position: absolute;
    top: 0;
    left: 0;
    width: 19%;
  }
  h2 {
    color: var(--darkGrey);
    font-size: 40px;
    font-weight: 800;
    padding-bottom: 37px;
    padding-top: 20px;
  }
  p {
    padding-bottom: 37px;
  }
}
.courses_learn-more {
  width: 60%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 18px;
  .learn-more_card {
    width: 205px;
    margin-right: 45px;
    display: flex;
    flex-direction: column;
    align-items: center;
    &:last-child {
      margin-right: 0px;
    }
    img {
      width: 100%;
      aspect-ratio: 1;
      padding-bottom: 15px;
      margin-top: 27px;
    }
    h4 {
      color: var(--text-xs);
      font-size: 22px;
      font-weight: 800;
      margin-bottom: 14px;
    }
  }
}
.rate-container {
  margin-top: -1px;
  background-image: url("../assets/svg/driving-triangle.svg");
  min-height: 500px;
  background-size: 100% 125px;
  background-repeat: no-repeat;
  background-position: top;
  .rate-card {
    padding-top: 58px;
    display: flex;
    flex-direction: column;
    align-items: center;
    border-radius: 10px;
    border-top: 8px solid var(--main-green);
    background-color: #fff;
    height: 400px;
    width: 33%;
    margin-right: 20px;
    box-shadow: 0px 25px 20px 0px rgba(155, 155, 155, 0.71);
    p {
      padding-top: 50px;
      color: var(--text-xs);
    }
    .circular {
      height: 200px;
      width: 200px;
      position: relative;
      .bar {
        position: absolute;
        height: 100%;
        width: 100%;
        background: var(--main-green);
        border-radius: 100%;
        clip: rect(0px, 200px, 200px, 100px);
        .progress {
          position: absolute;
          height: 100%;
          width: 100%;
          border-radius: 100%;
          clip: rect(0px, 200px, 200px, 100px);
          background: #fff;
        }
      }
      .number {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        z-index: 10;
        font-size: 18px;
        font-weight: 500;
        color: var(--main-green);
        span {
          color: var(--text-xs);
          font-size: 40px;
          font-weight: 700;
        }
      }

      .inner {
        position: absolute;
        z-index: 6;
        top: 50%;
        left: 50%;
        height: 160px;
        width: 160px;
        margin: -80px 0 0 -80px;
        background: #fff;
        border-radius: 100%;
      }
    }
  }
}

// animazione

.circle95 .left95 .progress {
  z-index: 1;
  animation: left95 2s linear both;
}
@keyframes left95 {
  100% {
    transform: rotate(180deg);
  }
}
.circle95 .right95 {
  transform: rotate(180deg);
  z-index: 3;
}
.circle95 .right95 .progress {
  animation: right95 2s linear both;
  animation-delay: 2s;
}
@keyframes right95 {
  100% {
    transform: rotate(160deg);
  }
}

// PROGRESS 100%

.circle100 .left100 .progress {
  z-index: 1;
  animation: left100 2s linear both;
}
@keyframes left100 {
  100% {
    transform: rotate(180deg);
  }
}
.circle100 .right100 {
  transform: rotate(180deg);
  z-index: 3;
}
.circle100 .right100 .progress {
  animation: right100 2s linear both;
  animation-delay: 2s;
}
@keyframes right100 {
  100% {
    transform: rotate(180deg);
  }
}
</style>
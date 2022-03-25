<template>
  <section id="instructor" class="container-fluid">
      <div class="container">
         <h2 class="instructor-title">Your Instructors</h2>
      </div>
    <div class="container info-wrapper">
      <div class="instructor-info">
       
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices
          auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.
        </p>
      </div>
        <div class="more-info">
          <button class="green_button">More about us</button>
        </div>
    </div>
    <div class="container card-wrapper">
      <div
        class="instructor-card"
        v-for="(instructor, i) in instructors"
        :key="i"
      >
        <img :src="instructor.picture" alt="" />

        <h4>{{ instructor.name }}</h4>
        <div class="social">
          <a :href="instructor.social[0]"><i class="fab fa-facebook-f"></i></a>
          <a :href="instructor.social[1]"><i class="fab fa-twitter"></i></a>
          <a :href="instructor.social[2]"><i class="fab fa-instagram"></i></a>
        </div>
        <p>{{ instructor.info }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      instructors: [
        {
          picture: require(`../assets/img/instructor-mikehart.jpg`),
          name: "Mike Hart",
          social: ["#", "#", "#"],
          info: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          picture: require(`../assets/img/instructor-johnsmith.jpg`),
          name: "Jhon Smith",
          social: ["#", "#", "#"],
          info: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
        {
          picture: require(`../assets/img/instructor-angelahart.jpg`),
          name: "Angela Hart",
          social: ["#", "#", "#"],
          info: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
#instructor {

  min-height: 700px;
  .instructor-title{
      color: var(--darkGrey);
      font-size: 40px;
padding-bottom:40px ;
  }
  .container {
    display: flex;
  }
  .info-wrapper{
  align-items: center;
  justify-content: space-between;
  padding-bottom: 88px;
      .instructor-info{
          width: 66.8%;
          p{    
              padding-top: 16px;
              font-size: 21px;
              font-weight: 700;
              
              color: var(--text-xs);
          }
      }
      .more-info{
                    padding:0 5px;

          width: 33%;
          button{
              width:100%;

          }
      }
  }

.card-wrapper{
    gap:10px;

.instructor-card {
  padding-top: 47px;
  display: flex;
  flex-direction: column;
  align-items: center;
  border-radius: 10px;
  border-top: 6px solid var(--main-green);
  background-color: #fff;
  height: 471px;
  width: 33%;
  box-shadow: 0px 25px 20px 0px rgba(155, 155, 155, 0.71);
  line-height: 2;
  &:nth-child(2){
      height: 484px;
      img{
          height: 203px;
      }
  }
  img {
    height: 193px;
    width: 302px;
  }
  h4 {
    color: var(--darkGrey);
    font-size: 24px;
    font-weight: 700;
    padding-top: 40px;
  
  }
  .social {
    display: flex;
    gap: 20px;
    a {
      color: var(--text-xs);
    }
  }
  p{  font-weight: 700;
      text-align: center;
       width: 70%;
      color: var(--text-xs);
      
      
  }
}
}
}
</style>
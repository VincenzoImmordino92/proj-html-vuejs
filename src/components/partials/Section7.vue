<script>


export default {
name:'Section7',

components:{
  
}
}
</script>

<template>
  <div class="container">
    <section class="company">
      <!--  -->
      <div class="box_team_members d-flex flex-column">

        <div class="box_team_text">
          <h5>team member</h5>
          <h1>our experts team members</h1>
        </div>
        <div class="carousel_team_member d-flex">
<!-- prima carta del team -->
          <div class="team_member_card">

            <div class="box_image">
              <img src="/public/img/team1.png" alt="">
            </div>

            <div class="box_text_member d-flex flex-column justify-content-center align-items-center">
              <h1>cristiano messi</h1>
              <span>Ceo/founder</span>
              <div class="social d-flex">
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
              </div>
            </div>
          </div>

<!-- seconda carta del team -->
          <div class="team_member_card">

            <div class="box_image">
              <img src="/public/img/team2.png" alt="">
            </div>

            <div class="box_text_member d-flex flex-column justify-content-center align-items-center">
              <h1>cristiano messi</h1>
              <span>Ceo/founder</span>
              <div class="social d-flex">
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
              </div>
            </div>
          </div>

<!-- terza carta del team -->
          <div class="team_member_card">

            <div class="box_image">
              <img src="/public/img/team3.png" alt="">
            </div>

            <div class="box_text_member d-flex flex-column justify-content-center align-items-center">
              <h1>cristiano messi</h1>
              <span>Ceo/founder</span>
              <div class="social d-flex">
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
              </div>
            </div>
          </div>

<!-- quarta carta del team -->
          <div class="team_member_card">

            <div class="box_image">
              <img src="/public/img/team4.png" alt="">
            </div>

            <div class="box_text_member d-flex flex-column justify-content-center align-items-center">
              <h1>cristiano messi</h1>
              <span>Ceo/founder</span>
              <div class="social d-flex">
                <a href="#"><i class="fa-brands fa-facebook"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
              </div>
            </div>
          </div>

          <div class="button_carousel">
            <button><i class="fa-solid fa-arrow-left-long"></i></button>
            <button><i class="fa-solid fa-arrow-right-long"></i></button>
          </div>
        </div>

        
        
      </div>
    </section>
  </div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;
.company{
  height: 100%;
  background-color: $color-bg-container-2-5-8-11;
  position: relative;
    .box_team_members{
      margin: 110px 0px;
      width: 100%;
      height: 100%;
      .box_team_text{
        width: 460px;
        h5{
          color: $color-text-btn;
          text-transform: capitalize;
        }
        h1{
          font-size: 3rem;
          font-weight: 700;
          letter-spacing:0.1px;
          text-transform: capitalize;
        }
      }
      .carousel_team_member{
        position: relative;
        .team_member_card{
          width: 300px;
          height: 400px;
          margin: 0px 10px;
          .box_image{
            height: 70%;
            img{
              width: 100%;
              height: 100%;
            }
          }
          .box_text_member{
            height: 30%;
            background-color: rgb(21, 34, 87);
            position: relative;
            h1{
              font-size: 1rem;
              text-transform: capitalize;
              font-weight: 700;
            }
            span{
              font-size: 1rem;
              text-transform: capitalize;
              font-weight: 700;
            }
            &:hover{
              background-color: $color-hover;
              color: $color-bg-container-2-5-8-11;
            }
            .social{
              position: absolute;
              top: -70px;
              a{
                display: inline-block;
                background-color: $color-bg-container-2-5-8-11;
                height: 40px;
                width: 40px;
                text-align: center;
                line-height: 40px;
                border-radius: 50%;
                margin: 5px;
                
                &:hover{
                  background-color:$color-text-btm-hover;
                }
                i{
                  color: $color-text;
                }
              }
            }
          }
        }
        .button_carousel{
          position: absolute;
          right: 15px;
          top:-60px;
          button{
          width: 40px;
          height: 40px;
          margin: 5px;
          border: none;
          border-radius: 50%;
            &:hover{
            color: $color-text;
            background-color: $color-text-btm-hover;
        }
      }
    }
      }
    } 
}
</style>
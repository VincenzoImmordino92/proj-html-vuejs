<script>


export default {
name:'Section6',

components:{
  
}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/public/img/v-bg.png" alt="">

    <div class="container">

      <section class="upcoming_match d-flex flex-column justify-content-center">

        <div class="upcoming_text">
          <h5>upcoming match</h5>
          <h1>keep eyes & manage upcoming battle</h1>
        </div>


        <div class="carosel_upcoming_card d-flex">
<!-- prima carta match view -->
          <div class="upcoming_card d-flex flex-column align-items-center">
            <div class="box_image">
              <img src="/public/img/m1.png" alt="">
            </div>
            <h1>Ninja Warrior Gaming</h1>
            <div class="social d-flex">
            <a href="#"><i class="fa-brands fa-youtube"></i></a>
            <a href="#"><i class="fa-solid fa-message"></i></a>
            </div>
            <h1>9.45</h1>
            <p>1st november, 2022</p>
            <button class="read_more">View More</button>
          </div>
<!-- seconda carta match view -->
          <div class="upcoming_card d-flex flex-column align-items-center">
            <div class="box_image">
              <img src="/public/img/m2.png" alt="">
            </div>
            <h1>Witch Gaming</h1>
            <div class="social d-flex">
            <a href="#"><i class="fa-brands fa-youtube"></i></a>
            <a href="#"><i class="fa-solid fa-message"></i></a>
            </div>
            <h1>9.45</h1>
            <p>1st november, 2022</p>
            <button class="read_more">View More</button>
          </div>
<!--  carta match view -->
          <div class="upcoming_card d-flex flex-column align-items-center">
            <div class="box_image">
              <img src="/public/img/m3.png" alt="">
            </div>
            <h1>skullg Gaming</h1>
            <div class="social d-flex">
            <a href="#"><i class="fa-brands fa-youtube"></i></a>
            <a href="#"><i class="fa-solid fa-message"></i></a>
            </div>
            <h1>9.45</h1>
            <p>1st november, 2022</p>
            <button class="read_more">View More</button>
          </div>

          <div class="button_carousel">
            <button><i class="fa-solid fa-arrow-left-long"></i></button>
            <button><i class="fa-solid fa-arrow-right-long"></i></button>
          </div>

        </div>
      </section>
    </div>
  </div>
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;

.bg_section{
  height: 1140px;
  position: relative;
  .bg_3{
    position: absolute;
    object-fit: cover;
    filter: opacity(0.4);
    height: 100%;
    width: 100%;
  }
  .upcoming_match{
  height: 1140px;
  width: 100%;
  .upcoming_text{
    width: 500px;
    z-index: 1;
    h5{
      color: $color-text-btn;
      font-weight: 500;
      text-transform: capitalize;
    }
    h1{
      font-weight: 700;
      text-transform: capitalize;
    }
  }
  .carosel_upcoming_card{
    z-index: 1;
    position: relative;
    .upcoming_card{
      height: 690px;
      width: 420px;
      background-color: $color-bg-box-squad-letters;
      border-radius: 10px;
      margin: 0px 10px;
      h1{
        font-size: 2rem;
        margin: 20px 0px;
        font-weight: 700;
        text-transform: capitalize;
      }
      p{
        font-weight: 700;
        text-transform: capitalize;
      }
      .box_image{
        width: 360px;
        height: 300px;
        border-radius: 15px;
        margin-top:30px ;
        padding-top: 30px;
        background-color: $color-bg-container-2-5-8-11;
        text-align: center;
        img{
          width: 80%;
          height: 80%;
          object-fit: contain;
        }
      }
      a{
        display: inline-block;
        background-color:$color-text-btn;
        height: 45px;
        width: 45px;
        text-align: center;
        line-height: 50px;
        border-radius: 50%;
        margin: 5px;
        i{
          color:$color-bg-container-2-5-8-11;
          &:hover{
          color:$color-text-btm-hover;
        }
        }
        &:hover{
          background-color: $color-bg-container-2-5-8-11;
        }
        
      }
      .read_more{
        padding: 15px 30px;
        border: none;
        background-color: $color-hover;
        border-radius: 5px;
        font-weight: 600;
        &:hover{
          background-color:$color-bg-container-2-5-8-11;
          color: $color-hover;  
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
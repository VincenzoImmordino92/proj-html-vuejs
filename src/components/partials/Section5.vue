<script>


export default {
name:'Section5',

components:{

}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/public/img/protfolio-vector.png" alt="">

    <div class="container">

      <section class="trending_games d-flex flex-column justify-content-center">
        <!-- testo iniziale trending -->
        <div class="trending_text_intro">
          <h5>trending games</h5>
          <h1>choose who is the best in world!</h1>
          
        </div>

        <!-- creazione card trending -->
      <div class="container_card d-flex">

        <div class="card_carosel_trending">
          <div class="box_image">
            <img src="/public/img/protfolio1.png" alt="">
          </div>
          <span>new</span>
          <div class="box_text d-flex justify-content-center">
            <div>
              <h1>assassin's creed</h1>
              <p>Lorem ipsum dolor sit</p>
            </div>
            <div class="box_play">
              <button class="play"><i class="fa-solid fa-play"></i></button>
            </div>
          </div>
        </div>

        <div class="card_carosel_trending">
          <div class="box_image">
            <img src="/public/img/protfolio2.png" alt="">
          </div>
          <span>new</span>
          <div class="box_text d-flex justify-content-center">
            <div>
              <h1>assassin's creed</h1>
              <p>Lorem ipsum dolor sit</p>
            </div>
            <div class="box_play">
              <button class="play"><i class="fa-solid fa-play"></i></button>
            </div>
          </div>
        </div>

        <div class="card_carosel_trending">
          <div class="box_image">
            <img src="/public/img/protfolio3.png" alt="">
          </div>
          <span>new</span>
          <div class="box_text d-flex justify-content-center">
            <div>
              <h1>assassin's creed</h1>
              <p>Lorem ipsum dolor sit</p>
            </div>
            <div class="box_play">
              <button class="play"><i class="fa-solid fa-play"></i></button>
            </div>
          </div>
        </div>

        <div class="card_carosel_trending">
          <div class="box_image">
            <img src="/public/img/protfolio4.png" alt="">
          </div>
          <span>new</span>
          <div class="box_text d-flex justify-content-center">
            <div>
              <h1>assassin's creed</h1>
              <p>Lorem ipsum dolor sit</p>
            </div>
            <div class="box_play">
              <button class="play"><i class="fa-solid fa-play"></i></button>
            </div>
          </div>
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
  height: 815px;
  background-color:$color-bg-box-squad-letters;
  position: relative;
  .bg_3{
    position: absolute;
    object-fit: cover;
    filter: opacity(0.4);
    height: 100%;
    width: 100%;
  }
  .trending_games{
    height: 815px;
    .trending_text_intro{
      width: 580px;
      h5{
        color: $color-text-btn;
        text-transform: capitalize;
      }
      h1{
        font-size: 3rem;
        font-weight: 700;
      }
    }
    .container_card{
      position: relative;
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
    
    .card_carosel_trending{
      width: 300px;
      height: 380px;
      z-index: 1;
      margin: 10px;
      position: relative;
      &:hover .box_text{
          background-color: $color-text-btm-hover;
        }
      span{
          position: absolute;
          width: 60px;
          height: 35px;
          background-color: $color-text-btn;
          z-index: 99;
          top: 0;
          text-align: center;
          line-height: 35px;
        }
      .box_image{
        width: 100%;
        height: 75%;
        
        img{
          width: 100%;
          height: 100%;
          z-index: 2;
          object-fit: cover;
        }
        
      }
      .box_text{
        height: 25%;
        background-color: rgb(21, 34, 87);
        padding: 20px;
        
        h1{
          font-size: 1.2rem;
          font-weight: 700;
        }
        p{
          text-transform:capitalize;
        }
        .play{
        width: 52px;
        height: 52px;
        border: none;
        background-color: $color-hover;
        border-radius: 50%;
        margin-left: 15px;
        &:hover{
          background-color: $color-bg-container-2-5-8-11;
          i{
            color:$color-text-btm-hover;
          }
        }
        i{
          font-size: 1.2rem;
          line-height: 21px;
          color:$color-bg-container-2-5-8-11;
        }
      }
      }
    }
  }
  }
}


/* .button_carousel{
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
    } */

</style>
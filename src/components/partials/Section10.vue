<script>


export default {
name:'Section10',

components:{
  
}
}
</script>

<template>
  <div class="container">
    <section class="news">
      <!--  -->
      <div class="box_news d-flex flex-column">

        <div class="box_news_text">
          <h5>latest news</h5>
          <h1>stay updated with ouur latest news articles</h1>
        </div>
        <div class="carousel_news d-flex">
<!-- prima card news -->
          <div class="card_news">
            <div class="box_image">
              <img src="/public/img/b1.png" alt="">
            </div>
            <div class="box_text_news d-flex flex-column justify-content-center align-items-center">
              <h1>ninja warrior gaming</h1>
              <span><i class="fa-brands fa-youtube"></i> by admin | <i class="fa-solid fa-calendar-days"></i> oct 25, 2022</span>
              <button class="read_more">read more <i class="fa-solid fa-arrow-right-long"></i> </button>
            </div>
          </div>

<!-- seconda card news -->
          <div class="card_news">
            <div class="box_image">
              <img src="/public/img/b2.png" alt="">
            </div>
            <div class="box_text_news d-flex flex-column justify-content-center align-items-center">
              <h1>ninja warrior gaming</h1>
              <span><i class="fa-brands fa-youtube"></i> by admin | <i class="fa-solid fa-calendar-days"></i> oct 25, 2022</span>
              <button class="read_more">read more <i class="fa-solid fa-arrow-right-long"></i> </button>
            </div>
          </div>

<!-- terza card news -->
          <div class="card_news">
            <div class="box_image">
              <img src="/public/img/b3.png" alt="">
            </div>
            <div class="box_text_news d-flex flex-column justify-content-center align-items-center">
              <h1>ninja warrior gaming</h1>
              <span><i class="fa-brands fa-youtube"></i> by admin | <i class="fa-solid fa-calendar-days"></i> oct 25, 2022</span>
              <button class="read_more">read more <i class="fa-solid fa-arrow-right-long"></i> </button>
            </div>
          </div>

<!-- quarta card news -->
          <div class="card_news">
            <div class="box_image">
              <img src="/public/img/b4.png" alt="">
            </div>
            <div class="box_text_news d-flex flex-column justify-content-center align-items-center">
              <h1>ninja warrior gaming</h1>
              <span><i class="fa-brands fa-youtube"></i> by admin | <i class="fa-solid fa-calendar-days"></i> oct 25, 2022</span>
              <button class="read_more">read more <i class="fa-solid fa-arrow-right-long"></i> </button>
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
.news{
  height: 100%;
  background-color: $color-bg-container-2-5-8-11;
  position: relative;
    .box_news{
      margin: 150px 0px;
      width: 100%;
      height: 100%;
      .box_news_text{
        width: 650px;
        margin-bottom: 50px;
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
      .carousel_news{
        position: relative;
        margin-bottom: 70px;
        .card_news{
          height: 510px;
          width: 310px;
          background-color: $color-bg-box-squad-letters;
          border-radius: 20px;
          margin: 10px;
          .box_image{
            height: 50%;
            width: 100%;
            img{
              height: 100%;
              width: 100%;
              object-fit: cover;
              border-radius: 20px 20px 0px 0px;
            }
          }
        }
        .box_text_news{
          padding: 15px;
          h1{
            font-size: 1.5rem;
            font-weight: 700;
            text-transform: capitalize;
            margin: 10px 0px;
          }
          span{
            text-transform: capitalize;
            margin: 10px 0px;
            i{
              color: $color-text-btn;
              margin: 20px 0px;
            }
          }
          .read_more{
            padding: 15px 30px;
            border: none;
            background-color: $color-hover;
            border-radius: 5px;
            font-weight: 600;
            &:hover{
              background-color: $color-bg-container-2-5-8-11;
              color: $color-text;
              i{
                color: $color-text;
              }
            }
            i{
              font-size: 1rem;
              color:$color-bg-container-2-5-8-11;
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



<script>


export default {
name:'Section9',

components:{
  
}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/public/img/shop-bg.png" alt="">

    <div class="container">
      <section class="gammer_shop d-flex flex-column justify-content-center">
        
        <div class="shop_text_intro">
          <h5>testimonials</h5>
          <h1>what our client say</h1>
        </div>

        <div class="carousel_shop d-flex">
<!-- prima car shop -->
          <div class="card_shop">
            <div class="box_image">
              <img src="/public/img/s1.png" alt="">
              <div class="social d-flex">
                <a href="#"><i class="fa-solid fa-eye"></i></a>
                <a href="#"><i class="fa-solid fa-cart-flatbed"></i></a>
                <a href="#"><i class="fa-solid fa-heart"></i></a>
              </div>
            </div>
            <div class="box_stars d-flex">
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
            </div>
            <h1>asus rog strix a53</h1>
            <span>$970.00</span>
            <span>$999.00</span>
          </div>
<!-- seconda card shop -->
          <div class="card_shop">
            <div class="box_image">
              <img src="/public/img/s2.png" alt="">
              <div class="social d-flex">
                <a href="#"><i class="fa-solid fa-eye"></i></a>
                <a href="#"><i class="fa-solid fa-cart-flatbed"></i></a>
                <a href="#"><i class="fa-solid fa-heart"></i></a>
              </div>
            </div>
            <div class="box_stars d-flex">
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
            </div>
            <h1>asus rog strix a53</h1>
            <span>$970.00</span>
            <span>$999.00</span>
          </div>
<!-- terza card shop -->
          <div class="card_shop">
            <div class="box_image">
              <img src="/public/img/s3.png" alt="">
              <div class="social d-flex">
                <a href="#"><i class="fa-solid fa-eye"></i></a>
                <a href="#"><i class="fa-solid fa-cart-flatbed"></i></a>
                <a href="#"><i class="fa-solid fa-heart"></i></a>
              </div>
            </div>
            <div class="box_stars d-flex">
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
            </div>
            <h1>asus rog strix a53</h1>
            <span>$970.00</span>
            <span>$999.00</span>
          </div>
<!-- quarta card shop -->
          <div class="card_shop">
            <div class="box_image">
              <img src="/public/img/s4.png" alt="">
              <div class="social d-flex">
                <a href="#"><i class="fa-solid fa-eye"></i></a>
                <a href="#"><i class="fa-solid fa-cart-flatbed"></i></a>
                <a href="#"><i class="fa-solid fa-heart"></i></a>
              </div>
            </div>
            <div class="box_stars d-flex">
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
              <i class="fa-solid fa-star-half-stroke"></i>
            </div>
            <h1>asus rog strix a53</h1>
            <span>$970.00</span>
            <span>$999.00</span>
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
  height: 770px;
  position: relative;
  .bg_3{
    position: absolute;
    object-fit: cover;
    filter: opacity(0.4);
    height: 100%;
    width: 100%;
  }
  .gammer_shop{
  height: 750px;
  width: 100%;
  .shop_text_intro{
    h5{
      color: $color-text-btn;
      text-transform: capitalize;
    }
    h1{
      font-size: 3rem;
      text-transform: capitalize;
      font-weight: 700;
    }
  }
  .carousel_shop{
    z-index: 1;
    position: relative;
    .card_shop{
      margin: 10px;
      .box_image{
        width: 300px;
        height: 260px;
        padding: 25px;
        border-radius: 10px;
        background-color: $color-bg-container-2-5-8-11;
        position: relative;
        &:hover a{
          display: inline-block;
        }
        img{
          width: 100%;
          height: 100%;
          object-fit: contain;
        }
        .social{
              position: absolute;
              bottom: 40%;
              left:50%;
              transform: translate(-50%, 100%);
              a{
                display: none;
                background-color:$color-bg-box-squad-letters;
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
      .box_stars{
        margin: 20px 0 ;
        i{
          font-size: 1.2rem;
        }
      }
      h1{
        font-size: 1.2rem;
        font-weight: 700;
      }
      span{
        padding: 5px 5px 0px 0px;
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
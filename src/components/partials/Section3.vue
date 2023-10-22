<script>


export default {
name:'Section3',

components:{
  
}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/public/img/v-bg.png" alt="">

    <div class="container">
      <section class="live_streaming d-flex justify-content-center align-items-center">
        <div class="row z-1">
          <div class="col">
            <img src="/public/img/v-1.png" alt="">
          </div>
          <div class="col flex-column">
            <h5>live streaming</h5>
            <h1>checkiut our live streaming</h1>
            <div class="box_carosel d-flex">
              <div class="button_carousel">
                <button><i class="fa-solid fa-arrow-left-long"></i></button>
                <button><i class="fa-solid fa-arrow-right-long"></i></button>
              </div>
              <div class="box_gaming">
                <img src="/public/img/v-small1.png" alt="">
                <h5>Call of deauty</h5>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eius, aspern</p>
              </div>
              <div class="box_gaming">
                <img src="/public/img/v-small2.png" alt="">
                <h5>assassin's creed</h5>
                <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Eius, aspern</p>
              </div>

            </div>
          </div>
        </div>
        
      </section>
    </div>
  </div>
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;

.bg_section{
  height: 750px;
  position: relative;
  .bg_3{
    position: absolute;
    object-fit: cover;
    filter: opacity(0.4);
    height: 100%;
    width: 100%;
  }
  .live_streaming{
  height: 750px;
  width: 100%;
  img{
    width: 635px;
    height: 470px;
    object-fit: contain;
  }
  h5{
    color: $color-text-btn;
    text-transform: capitalize;
  }
  h1{
    font-size: 3rem;
    text-transform: capitalize;
    font-weight: 700;
  }
  .box_carosel{
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
    .box_gaming{
      h5{
        color: $color-text;
        font-weight: 600;
        padding: 5px 0;
      }
      p{
        font-size: 0.8rem;
        font-weight: 500;
      }
    }
    img{
      width: 300px;
      height: 210px;
    }
  }
  }
}

</style>
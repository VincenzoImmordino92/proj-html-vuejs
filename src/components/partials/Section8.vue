<script>


export default {
name:'Section5',

components:{

}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/public/img/test-group.png" alt="">

    <div class="container">

      <section class="testimonials d-flex flex-column justify-content-center">
        <!-- testo iniziale trending -->
        <div class="testimonials_text_intro">
          <h5>testimonials</h5>
          <h1>what our client say</h1>
          
        </div>

        <!-- creazione card trending -->
      <div class="container_card d-flex">

        <div class="card_client">
          <div class="box_image">
            <img src="/public/img/test1.png" alt="">
          </div>
        </div>

        <div class="card_client">
          <div class="box_image">
            <img src="/public/img/test2.png" alt="">
          </div>
        </div>

        <div class="card_client">
          <div class="box_image">
            <img src="/public/img/test3.png" alt="">
          </div>
        </div>

        <div class="card_client">
          <div class="box_image">
            <img src="/public/img/test4.png" alt="">
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
  .testimonials{
    height: 800px;
    
    .testimonials_text_intro{
      width: 580px;
      margin: 20px 0px;
      h5{
        text-align: center;
        color: $color-text-btn;
        text-transform: capitalize;
      }
      h1{
        text-align: center;

        font-size: 3rem;
        font-weight: 700;
      }
    }
    .container_card{
      position: relative;
      .card_client{
        padding: 5px;
        .box_image{
          width: 320px;
          height: 400px;
          background-color: rgb(174, 149, 207);

          img{
            width: 100%;
            height: 100%;
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
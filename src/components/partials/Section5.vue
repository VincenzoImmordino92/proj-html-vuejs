<script>
import Card_trending from './Card_trending.vue'
import {card_trending_section5} from '../../data/card_general'

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';
  // Import Swiper styles
  import 'swiper/css';
  import 'swiper/css/navigation';
  

  // import required modules
  import { Navigation } from 'swiper/modules';

export default {
name:'Section5',
data(){
  return{
    card_trending_section5
  }
},
components:{
  Card_trending,
  Swiper,
  SwiperSlide,
},
setup() {
      return {
        modules: [Navigation],
        
      };
    },
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/img/protfolio-vector.png" alt="">

    <div class="container overflow-hidden">

      <section class="trending_games d-flex flex-column justify-content-center z-1">
        <!-- testo iniziale trending -->
        <div class="trending_text_intro">
          <h5>trending games</h5>
          <h1>choose who is the best in world!</h1>
          
        </div>

        <!-- creazione card trending -->
      <div class="container_card">

          <swiper
            :slidesPerView="4"
            :spaceBetween="5"
            :navigation="true"
            :centeredSlides="false"
            :modules="modules"
            class="mySwiper"
          >

            <swiper-slide v-for="(card,index) in card_trending_section5" :key="index">
              <Card_trending :item="card"/>
            </swiper-slide>

          </swiper>
        

          <!-- <div class="button_carousel">
            <button ><i class="fa-solid fa-arrow-left-long"></i></button>
            <button ><i class="fa-solid fa-arrow-right-long"></i></button>
          </div>  -->
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
    
    
  }
  }
} 

</style>

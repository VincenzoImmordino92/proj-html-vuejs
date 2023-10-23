<script>

import {card_match_section4} from '../../data/card_general';
import Card_match from './Card_match.vue';

export default {
name:'Section4',

data(){
    return{
      card_match_section4
  }
},
components:{
  Card_match
}
}
</script>

<template>
  <div class="container">
    <section class="company">
      
      <div class="box_upcoming_match d-flex flex-column align-items-center">
        <div class="box_match_text">
          <h5>trending battle</h5>
          <h1>upcoming match</h1>
          <ul class="d-flex justify-content-center">
            <li><a href="#">all</a></li>
            <li><a href="#">pubg</a></li>
            <li><a href="#">cod</a></li>
            <li><a href="#">ac</a></li>
            <li><a href="#">mcx</a></li>
          </ul>
        </div>
        <Card_match v-for="(card,index) in card_match_section4" :key="index" :item="card" />
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
    .box_upcoming_match{
      margin: 110px 0px;
      width: 100%;
      height: 100%;
      .box_match_text{
        h5{
          text-align: center;
          color: $color-text-btn;
          text-transform: capitalize;
        }
        h1{
          font-size: 3rem;
          font-weight: 700;
          letter-spacing:0.1px;
          text-transform: capitalize;
        }
        ul{
          padding: 20px 0px;
          li{
            padding: 10px 20px;
            text-transform: capitalize;
            a{
              color: $color-text;
              text-decoration: none;
              font-weight: 700;
              &:hover{
                color: $color-text-btm-hover;
                
              }
            }
          }
        }
      }
  } 
}
</style>
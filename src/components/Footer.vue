<script>

import Box_letters from './partials/Box_letters.vue';
import { menuHeader_footer } from '../data/menu_header_footer';
export default {
Name:'Footer',
data(){
  return{
    menuHeader_footer
  }
},
  components:{
    Box_letters
  }
}

</script>

<template>
<div class="bg-footer">
  
  <img class="bg" src="/img/footer-bg.png" alt="">
  <div class="container padding_custom">
    <Box_letters /> 
    <!-- footer top -->
    <div class="footer-top d-flex justify-content-between align-items-center border-bottom">
      
        <div class="box_image">
          <img src="/public/img/menulogo.png" alt="logo">
        </div>
      
        <nav>
          <ul class="d-flex justify-content-end">
            <li v-for="(item, index) in menuHeader_footer" :key="index">
              <a :href="item.href">{{ item.text }}</a>
            </li>
            
          </ul>
        </nav>
    </div>

    <!-- fotter bottom -->
    <div class="footer-bottom d-flex justify-content-between align-items-center pt-3">
      
        <span>Copyrigt &copy; RaxG | Designed by <span>NextGenerationDev</span></span>
      
      
        <div class="social d-flex justify-content-end">
        <a href="#"><i class="fa-brands fa-facebook"></i></a>
        <a href="#"><i class="fa-brands fa-twitter"></i></a>
        <a href="#"><i class="fa-brands fa-linkedin"></i></a>
        <a href="#"><i class="fa-brands fa-instagram"></i></a>
      </div>
      
    </div>
  </div>

</div>
</template>

<style lang="scss" scoped>

@use '../scss/partials/vars' as *;

.bg-footer{
  position: relative;
  height: 466px;
  .bg{
    position: absolute;
    object-fit: cover;
    z-index: -1;
    filter: opacity(0.4) ;
    width: 100%;
  }
  
  .padding_custom{
    padding-top: 180px;    
  }
  .footer-top{
    padding: 35px 0px;
  }
nav{
  ul{
    li{
      padding: 0px 10px;
      a{
        text-transform: uppercase;
        font-weight: 700;
        color:$color-text;
        text-decoration: none;
        &:hover{
          color: $color-text-btm-hover;
        }
      }
    }
  }
}

  .social{
      a{
        display: inline-block;
        background-color: $color-bg-container-2-5-8-11;
        height: 45px;
        width: 45px;
        text-align: center;
        line-height: 50px;
        border-radius: 50%;
        margin: 0px 7px;
        &:hover{
          background-color:$color-text-btm-hover;
        }
        i{
          color: $color-text;
        }
      }
    }
  
}


</style>
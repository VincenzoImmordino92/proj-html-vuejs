<script>

import {menuHeader} from '../data/menu_header_footer'

export default {
Name:'Header',
data(){
  return{
    menuHeader
  }
}
}

</script>

<template>
  <div class="banner_1">
    <div class="container">
        <div class="row justify-content-between align-items-center">
          <!-- Logo -->
          <div class="col">
            <div class="box_image">
              <img src="/public/img/menulogo.png" alt="menulogo">
            </div>
          </div>
          <!-- Menu -->
          <div class="col">
            <nav>
              <ul class="d-flex">
            <!-- menu da ciclare creando un array di con le informazioni dentro(credo) -->
                <li v-for="(item, index) in menuHeader" :key="index">
                  <a :href="item.href">{{ item.text }}<i :class="item.arrow"></i></a>
                </li>
              </ul>
            </nav>
          </div>
          <!-- Search/Shop -->
          <div class="col">
            <div class="btn_custom d-flex justify-content-center">
              <button><i class="fa-solid fa-magnifying-glass"></i></button>
              <button><i class="fa-solid fa-bag-shopping"></i><span>0</span></button>
            </div>
          </div>
        </div>
        <!-- Welcome to raxg -->
    <div class="welcome text-center">
      <h5>welcome to raxg</h5>
      <h1>are you ready for your next challenge?</h1>
      <div class="box_button">
        <button class="read_more">read more <i class="fa-solid fa-arrow-right-long"></i> </button>
        <button class="play"><i class="fa-solid fa-play"></i></button>
      </div>
    </div>
    </div>
    <!-- Container Social -->
    <div class="container_custom d-flex align-items-center">
      <div class="social d-flex flex-column">
        <a href="#"><i class="fa-brands fa-facebook"></i></a>
        <a href="#"><i class="fa-brands fa-twitter"></i></a>
        <a href="#"><i class="fa-brands fa-linkedin"></i></a>
        <a href="#"><i class="fa-brands fa-instagram"></i></a>
      </div>
    </div>

  </div>

</template>

<style lang="scss" scoped>

@use '../scss/partials/vars' as *;

.banner_1{
  background-image: url('/img/banner1.png');
  width: 100%;
  height: 900px;
  background-size: cover;
  background-repeat: no-repeat;
  position: relative;
  .container{
    nav{
      width: 100%;
      ul{
        li{
          padding: 0px 10px;
          width: 20%;
          flex-shrink: 0;
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
    .btn_custom{
      button{
        width: 40px;
        height: 40px;
        border: none;
        margin: 10px;
        border-radius: 50%;
        position: relative;
        i{
          color: $color-bg-box-squad-letters;
        }
        span{
          position: absolute;
          color: $color-text;
          font-size: 1rem;
          line-height: 30px;
          width: 30px;
          height: 30px;
          top:-10px;
          right: -10px;
          border-radius: 50%;
          background-color:$color-bg-box-hover;
        }
      }
    }
  .welcome{
    position: absolute;
    width: 1030px;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    h5{
      color: $color-text-btn;
      text-transform: uppercase;
    }
    h1{
      text-transform: uppercase;
      font-weight: 700;
      font-size: 4.4rem;
    }
    .box_button{
      margin-top: 40px;
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
      .play{
        width: 58px;
        height: 58px;
        border: none;
        background-color: $color-hover;
        border-radius: 50%;
        margin-left: 15px;
        &:hover{
          background-color: $color-bg-container-2-5-8-11;
          i{
            color: $color-text;
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
  .container_custom{
    width: 100%;
    height: 100%;
    padding-left: 145px;
    
    .social{
      margin-bottom:180px;
      a{
        display: inline-block;
        background-color: $color-bg-container-2-5-8-11;
        height: 45px;
        width: 45px;
        text-align: center;
        line-height: 50px;
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

</style>
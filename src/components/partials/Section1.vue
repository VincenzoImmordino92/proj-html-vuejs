<script>
import Box_squad from './Box_squad.vue';

export default {
name:'Section1',

components:{
  Box_squad
}
}
</script>

<template>
  <div class="container">
    <section class="company">
      <Box_squad />
      <div class="box_best_gaming d-flex">
        <div class="box_image">
          <img class="shape1" src="/public/img/shape1.png" alt="shape1">
          <img src="/public/img/exprince.jpg" alt="exprice">
          <img class="shape2" src="/public/img/shape2.png" alt="shape2">
          <img class="shape_ex" src="/public/img/exprience-shape.png" alt="">
        </div>
        <div class="box_text d-flex flex-column">
          <h6>12 year experience</h6>
          <h1>we are the best gaming company</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis natus magni magnam eum libero repellat cum architecto dolor quae fuga aliquid autem illum commodi, aliquam dignissimos officia error quos maiores?ibero repellat cum architecto dolor quae fuga aliquid autem illum commodi.</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id labore laudantium ab pariatur enim neque.</p>
          <ul>
            <li><span><i class="fa-solid fa-check"></i></span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</li>
            <li><span><i class="fa-solid fa-check"></i></span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</li>
            <li><span><i class="fa-solid fa-check"></i></span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</li>
            <li><span><i class="fa-solid fa-check"></i></span>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</li>
          </ul>
          <div class="box_button">
            <button class="read_more">read more <i class="fa-solid fa-arrow-right-long"></i> </button>
            <button class="play"><i class="fa-solid fa-play"></i></button>
          </div>
        </div>
        
      </div>
    </section>
  </div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;
.company{
  height: 1100px;
  background-color: $color-bg-container-2-5-8-11;
  position: relative;
  
    .box_best_gaming{
      padding-top: 320px;
      width: 100%;
      height: 100%;
      .box_image{
        position: relative;
        margin-right: 70px;
        padding: 40px 0px;
        img{
          z-index: 1;
        }
        .shape1, .shape2, .shape_ex{
          position: absolute;
          z-index: 0;
        }
        .shape1{
          top: -45px;
          left: -45px;
        }
        .shape2{
        bottom: 130px;
          right: -40px;
        }
        .shape_ex{
          left: 0px;
        }
      }
      .box_text{
        width: 50%;
        h6{
          color: $color-text-btn;
          text-transform: capitalize;
          margin-bottom: 20px;
        }
        h1{
          font-size: 3rem;
          font-weight: 700;
          text-transform: capitalize;
          margin-bottom: 20px;
        }
        ul{
          padding: 0px;
          li{
            margin: 25px 0px;
            font-weight: 600;
            span{
              display: inline-block;
              border:1px solid $color-text-btn;
              width:25px;
              height:25px;
              border-radius: 50%;
              text-align: center;
              margin-right: 10px;
              i{
                font-size: 0.8rem;
                color:$color-text-btn;

              }
            }
          }
        }
        .box_button{
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
}
</style>
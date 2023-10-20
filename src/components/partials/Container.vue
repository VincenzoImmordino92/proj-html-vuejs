<script>
import Box_squad from './Box_squad.vue';

export default {
name:'Container',

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
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis natus magni magnam eum libero repellat cum architecto dolor quae fuga aliquid autem illum commodi, aliquam dignissimos officia error quos maiores?</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Id labore laudantium ab pariatur enim neque.</p>

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
        img{
          z-index: 1;
        }
        .shape1,.shape2,.shape_ex{
          position: absolute;
        }
        .shape1{
          top: -45px;
          left: -45px;
        }
        .shape2{
          bottom: -45px;
          
        }
      }
      .box_text{
        width: 50%;
      }
  } 
}
</style>
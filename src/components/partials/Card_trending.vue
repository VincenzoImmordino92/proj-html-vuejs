<script>
export default {
name: 'Card_trending',
props:{
  item:Object,
}
}
</script>


<template>
  <div>
    <div class="card_carosel_trending">
      <div class="box_image">
        <img :src="item.img" alt="">
      </div>
      <span>new</span>
      <div class="box_text d-flex justify-content-center">
        <div>
          <h1>{{ item.name }}</h1>
          <p>{{ item.text }}</p>
        </div>
        <div class="box_play">
          <button class="play"><i class="fa-solid fa-play"></i></button>
        </div>
      </div>
    </div>

  </div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as*;

.card_carosel_trending{
      width: 300px;
      height: 380px;
      z-index: 1;
      margin: 10px;
      position: relative;
      &:hover .box_text{
          background-color: $color-text-btm-hover;
        }
      span{
          position: absolute;
          width: 60px;
          height: 35px;
          background-color: $color-text-btn;
          z-index: 99;
          top: 0;
          text-align: center;
          line-height: 35px;
        }
      .box_image{
        width: 100%;
        height: 75%;
        
        img{
          width: 100%;
          height: 100%;
          z-index: 2;
          object-fit: cover;
        }
        
      }
      .box_text{
        height: 25%;
        background-color: rgb(21, 34, 87);
        padding: 20px;
        
        h1{
          font-size: 1.2rem;
          font-weight: 700;
        }
        p{
          text-transform:capitalize;
        }
        .play{
        width: 52px;
        height: 52px;
        border: none;
        background-color: $color-hover;
        border-radius: 50%;
        margin-left: 15px;
        &:hover{
          background-color: $color-bg-container-2-5-8-11;
          i{
            color:$color-text-btm-hover;
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
</style>
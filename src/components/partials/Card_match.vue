<script>

export default {
  name:'Card_match',
  
  props:{
    item:Object,
  }
}

</script>


<template>

  <div class="box_match d-flex justify-content-between align-items-center">

<!-- prima carta sfida -->
<div class="first_card d-flex flex-column">
  <div class="box_image_vs">
    <img :src="item.img1" :alt="item.name1">
  </div>
  <div class="box_text_vs d-flex flex-column justify-content-center">
    <h5>{{ item.nationality1 }}</h5>
    <h1>{{ item.name1 }}</h1>
  </div>
</div>

<!-- carta sfida VS -->
<div class="vs_card mx-3 d-flex justify-content-center align-items-center">
  <h1>vs</h1>
</div>

<!-- seconda carta sfida -->
<div class="second_card d-flex flex-column">
  <div class="box_image_vs">
    <img :src="item.img2" :alt="item.name2">
  </div>
  <div class="box_text_vs d-flex flex-column justify-content-center">
    <h5>{{ item.nationality2 }}</h5>
    <h1>{{ item.name2 }}</h1>
  </div>
</div>

<!-- box text content -->
<div class="vs_text">
  <h1>{{ item.titleGame }}</h1>
  <p>{{ item.text }}</p>
</div>

<!-- card date match -->
<div class="date_vs d-flex flex-column justify-content-center align-items-center">
  <h1>{{ item.time }}</h1>
  <p>{{ item.date }}</p>
  <div class="social d-flex">
  <a href="#"><i class="fa-brands fa-youtube"></i></a>
  <a href="#"><i class="fa-solid fa-message"></i></a>
  </div>
</div>
</div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;

.box_match{
        width: 100%;
        height: 360px;
        background-color:$color-bg-box-squad-letters;
        border: 1px solid $color-text-btn;
        padding: 25px;
        border-radius: 10px;
        margin: 15px 0;
        .first_card, .second_card{
          height: 280px;
          width: 200px;
          background-color: $color-bg-container-2-5-8-11;
          border-radius: 10px;
          margin: 5px;
          .box_image_vs{
            height: 65%;
            padding: 20px;
            img{
              width: 100%;
              height: 100%;
              object-fit: contain;
            }
          }
          .box_text_vs{
            height: 35%;
            background-color: rgb(21, 34, 87);
            border-radius: 0px 0px 10px 10px;
            padding: 5px 10px;
            h5{
              color: $color-text-btn;
              font-size: 1rem;
              text-transform: capitalize;
            }
            h1{
              font-size: 1.38rem;
              font-weight: 700;
              text-transform: capitalize;
            }
          }
        }
        .vs_card{
          height: 140px;
          width: 130px;
          background-color: $color-bg-container-2-5-8-11;
          border-radius: 10px;
          h1{
            color: $color-text-btn;
          }
        }
        .vs_text{
          width: 450px;
          padding: 0px 30px;
          h1{
            font-size: 1.85rem;
            letter-spacing: 0.01px;
            font-weight: 700;
            text-transform: capitalize;
          }
        }
        .date_vs{
          width: 185px;
          height: 190px;
          background-color: $color-bg-container-2-5-8-11;
          border-radius: 10px;
          a{
        display: inline-block;
        background-color:$color-text-btn;
        height: 45px;
        width: 45px;
        text-align: center;
        line-height: 50px;
        border-radius: 50%;
        margin: 5px;
        i{
          color:$color-bg-container-2-5-8-11;
        }
      }&:hover{
        background-color:$color-text-btm-hover;
        a{
          background-color:$color-bg-container-2-5-8-11;
          i{
            color: $color-text;
          }
      }
          }
        }&:hover{
          background-color: $color-bg-box;
          border: none;
        }
        }
</style>
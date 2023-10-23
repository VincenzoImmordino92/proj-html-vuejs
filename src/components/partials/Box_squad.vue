<script>
import { image_squad } from '../../data/image_squad';

export default {
name:'Box_squad',
data(){
  return{
    image_squad
  }
}
}
</script>

<template>
  <div class="box_squad">
    <ul>
      <li v-for="(img, index) in image_squad" :key="index">
        <img :src="img.img" :alt="img.text">
      </li>
    </ul>
  </div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;


.box_squad{
height: 230px;
width: 100%;
border-radius: 10px;
background-color: $color-bg-box-squad-letters;
position: absolute;
top: -10%;
  ul{
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    li{
      padding: 40px 25px;
      img{
        width: 100%;
        object-fit: contain;
      }
    }
  }
}
</style>
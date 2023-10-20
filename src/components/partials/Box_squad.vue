<script>
export default {
name:'Box_squad'
}
</script>

<template>
  <div class="box_squad">
    <ul>
      <li><img src="/img/1.png" alt="ninja"></li>
      <li><img src="/img/2.png" alt="for the king"></li>
      <li><img src="/img/3.png" alt="skullg"></li>
      <li><img src="/img/4.png" alt="panda"></li>
      <li><img src="/img/5.png" alt="witch"></li>
      <li><img src="/img/6.png" alt="astro"></li>
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
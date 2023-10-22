<script>


export default {
name:'Section3',

components:{
  
}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_3" src="/public/img/v-bg.png" alt="">

    <div class="container">
      <section class="live_streaming d-flex ">
        dscdcercer
        
      </section>
    </div>
  </div>
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;

.bg_section{
  height: 750px;
  position: relative;
  .bg_3{
    position: absolute;
    object-fit: cover;
    filter: opacity(0.4);
    height: 100%;
    width: 100%;
  }
  .live_streaming{
  height: 900px;
  width: 100%;
  }
}

</style>
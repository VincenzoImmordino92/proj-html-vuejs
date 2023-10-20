<script>
export default {
name:'Box_letters'
}
</script>

<template>
  <div class="box_letters d-flex justify-content-between align-items-center">
    <h1>our news letter</h1>
    <div>
      <div class="email_container">
        <i class="fa-solid fa-message"></i>
        <form>
          <input type="text" class="custom" placeholder="Enter Your Email">
          <button class="" type="button">Subscrive</button>
        </form>
        
      </div>
      
    </div>
  </div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;


.box_letters{
height: 230px;
width: 1295px;
border-radius: 10px;
background-color: $color-bg-box-squad-letters;
position: absolute;
top: -25%;
  h1{
    margin-left: 40px;
    text-transform: capitalize;
    font-size: 2.1rem;
    font-weight: 700;
  }
  .custome{
    background-color: $color-bg-container-2-5-8-11;
  }
  .email_container{
    width: 500px;
    height: 100px;
    background-color: $color-bg-container-2-5-8-11;
    border-radius:25px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    i{
      color: $color-text-btm-hover;
    }
      input{
        border: none;
      }
      button{
        border:none;
        border-radius: 20px;
        padding: 10px 15px;
        background-color: $color-text-btm-hover;
      }
  }
}
</style>
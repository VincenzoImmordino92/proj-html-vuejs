<script>


export default {
name:'Section2',

components:{

}
}
</script>

<template>
  <div class="bg_section">
    <img class="bg_2" src="/public/img/Vector.png" alt="">

    <div class="container">
      <section class="gaming d-flex ">
        <div class="row justify-content-center align-items-center">
          <div class="col w-50">
            <h6>our extrem feature</h6>
            <h1>the best gaming arena on the world!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Error tenetur quisquam placeat fugiat nam consectetur libero aperiam a reprehenderit minus.</p>
          </div>
          <div class="col w-50">
            <!-- Card Info-gaming 1 -->
            <div class="cards_wrap d-flex flex-wrap">
              <div class="card_custom d-flex flex-column justify-content-center align-items-center text-center">

                <div class="circle d-flex justify-content-center align-items-center">
                  <img src="/public/img/feature1.png" alt="">
                </div>

                <h5>live streaming</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>

              </div>
            <!-- Card Info-gaming 2 -->
              <div class="card_custom d-flex flex-column justify-content-center align-items-center text-center">

                <div class="circle d-flex justify-content-center align-items-center">
                  <img src="/public/img/feature2.png" alt="">
                </div>

                <h5>gaming news</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>

              </div>
            <!-- Card Info-gaming 3 -->
              <div class="card_custom d-flex flex-column justify-content-center align-items-center text-center">

                <div class="circle d-flex justify-content-center align-items-center">
                  <img src="/public/img/feature3.png" alt="">
                </div>

                <h5>great tournament</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>

              </div>
            <!-- Card Info-gaming 4 -->
              <div class="card_custom d-flex flex-column justify-content-center align-items-center text-center">

                <div class="circle d-flex justify-content-center align-items-center">
                  <img src="/public/img/feature4.png" alt="">
                </div>

                <h5>award ceremony</h5>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing.</p>
                
              </div>

            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<style lang="scss" scoped>

@use '../../scss/partials/vars' as *;

.bg_section{
  height: 900px;
  background-color:$color-bg-box-squad-letters;
  position: relative;
  .bg_2{
    position: absolute;
    object-fit: cover;
    filter: opacity(0.4);
    height: 100%;
    width: 100%;
  }
  
  .gaming{
  height: 900px;
  width: 100%;
    h6{
      color: $color-text-btn;
      text-transform: capitalize;
    }
    h1{
      font-size: 2.8rem;
      text-transform: capitalize;
      font-weight: 700;
    }
    .cards_wrap{
      .card_custom{
        height: 315px;
        width: 300px;
        background-color: $color-hover;
        color:$color-bg-box-squad-letters;
        padding: 10px;
        margin: 9px;
        border-radius: 20px;
        z-index: 1;
        &:nth-child(2){
          background-color: $color-bg-box;
          color: $color-text;
        }
        &:nth-child(3){
          background-color: $color-bg-box;
          color: $color-text;
        }
        h5{
          font-weight: 700;
          text-transform: capitalize;

        }
        .circle{
          width: 100px;
          height: 100px;
          border-radius: 50%;
          background-color: $color-bg-box-squad-letters;
          margin-bottom: 20px;
          img{
            width: 60px;
            height: 60px;
          }
        }
      }
    }
  }
}

</style>
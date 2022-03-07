<template>
  <section id="jumbotron" >
    <div class="container p-5 position-relative">
    <img class="position-absolute kid_01" src="../assets/images/slider_slide2_img1.png" alt="">
    <img class="position-absolute kid_02" src="../assets/images/slider_slide2_img2.png" alt="">
    <img class="position-absolute cubes" src="../assets/images/slider_icon16.png" alt="">
    <img class="position-absolute drawing" src="../assets/images/slider_icon14.png" alt="">
    <img class="position-absolute brush" src="../assets/images/slider_icon11.png" alt="">
    <img class="position-absolute train" src="../assets/images/slider_icon12.png" alt="">
    <img class="position-absolute potion" src="../assets/images/slider_icon13.png" alt="">
      <div class="row">
        <div class="col py-5 col-5 flex-column">
          <div class="text-box text-center">
            <h3 class="indie_flower text-start prim">Friendly Atmosphere</h3>
            <h3 class="fw-bold text-start seco">Welcoming Place</h3>
            <h3 class="fw-lighter text-start seco">For Every Child</h3>
            <button class="ms_btn_primary d-block">BUY THIS THEME NOW</button>
          </div>
        </div>
            <div class="slider-progress text-center mt-5">
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
            </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
    name: "MyJumbotron",
    data(){
      return{
        sliderImages: [
          {

          },
        ]
      }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

#jumbotron{
  background-image: url('../assets/images/slider_slide2_background.png');
  background-size: contain;

  .text-box{
    width: min-content;
    margin: auto;
    white-space: nowrap;
  }

  .indie_flower{
    font-family: "Indie Flower";
  }

.slider-button{
  border: 1px solid $primaryColor;
  &:hover{
    cursor: pointer;
  }
  &:active{
    transform: translateY(-50%);
    cursor: pointer;
    transition: transform 0.3s;
  }
}
  
}


// Posizionamento immagini con absolute 


  .kid_01{
    top: -100px;
    right: 13rem;
    transform: scale(0.6);
    z-index: 2;
  }

  .kid_02{
    top: -59px;
    right: 1rem;
    transform: scale(0.55);
    z-index: 1;
  }

  .cubes{
    left: 19rem;
    top: 0;
    transform: scale(0.6);
  }
 
  .drawing{
    left: 23rem;
    top: 4rem;
    transform: scale(0.6);
  }
 
  .brush{
    left: 25rem;
    top: 0;
    transform: scale(0.6);
  }
 
  .train{
    left: 28rem;
    top: 3.5rem;
    transform: scale(0.6);
  }
 
  .potion{
    left: 32rem;
    top: 0;
    transform: scale(0.6);
  }
 
 
</style>
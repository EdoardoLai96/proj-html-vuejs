<template>
  <section id="mygallery" class="d-flex align-items-center">
      <div class="container">
        <div class="row">
          <div class="col py-5">
            <div class="img_box my-3">
              <img class="quote" src="../assets/images/quote_alt.png" alt="">
            </div>
              <p class="text-white fs-1 fw-lighter text-center">I have to say that I have 2 children ages 5 and 2 and have used various daycare's in Kindergartens and this is by far the very best I have ever used.</p>
              <div class="text-white text-center">_____</div>
              <div class="quote_name text-center text-white my-2">Cecil J. Kirk</div>
              <div class="slider-progress text-center mt-5">
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
                <div class="slider-button d-inline-block mx-1"> </div>
              </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "MyGallery"

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

#mygallery{
  background-image: url('../assets/images/parallax_02.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;

  .img_box{
    border: 2px solid white;
    border-radius: 50%;
    padding: 1rem;
    width: min-content;
    margin: auto;
  }

  
}
 
 
</style>
<template>
  <section id="mygallery" class="d-flex align-items-center position-relative">
    <img class="position-absolute active_img_slider" :src="galleryPics[active].url" alt="">
      <div class="container">
        <div class="row mx-5">
          <div class="col py-5">
            <div class="img_box my-3">
              <img class="quote" src="../assets/images/quote_alt.png" alt="">
            </div>
              <p class="text-white fs-1 fw-lighter text-center">{{galleryPics[active].review}}</p>
              <div class="text-white text-center">_____</div>
              <div class="quote_name text-center text-white my-2">{{galleryPics[active].customer_name}}</div>
              <div class="slider-progress text-center mt-5">
                <div v-for="(slider_button , index) in galleryPics" :key="index" class="slider-button d-inline-block mx-1" :class="[index == active? 'active_slider_button' : '']"> </div>
              </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "MyGallery",
    data(){
      return{
        galleryPics : [
          {
            url: "../slider_gallery-images/blog_09-1024x614.jpg",
            review: "'The way I see it, if you’re gonna build a time machine into a car, why not do it with some style?'",
            customer_name:"Doc Brown"
          },
          {
            url: "../slider_gallery-images/blog_08-1024x614.jpg",
            review: "'It Takes Two To Lie: One To Lie, And One To Listen.'",
            customer_name:"Homer J. Simpson"

          },
          {
            url: "../slider_gallery-images/parallax_02.jpg",
            review: "'I have to say that I have 2 children ages 5 and 2 and have used various daycare's in Kindergartens and this is by far the very best I have ever used.'",
            customer_name:"Cecil J.Kirk"

          },
          {
            url: "../slider_gallery-images/blog_10-1024x614.jpg",
            review: "'Remember, with great power comes great responsibility.'",
            customer_name:"Ben Parker"

          },
          {
            url: "../slider_gallery-images/gallery_01.jpg",
            review: "'I am your Father Luke'",
            customer_name:"Darth Vather"

          },
          {
            url: "../slider_gallery-images/gallery_02.jpg",
            review: "'Look to my coming, at first light, on the fifth day. At dawn, look to the East'",
            customer_name:"Gandalf"
          },
        ],
        active: 0,
        intervalId1: ""
      }
      
    },
    methods:{

      makeActive(){
        if(this.active < this.galleryPics.length ){
          this.active++
        }if(this.active == this.galleryPics.length ){
          this.active = 0
        }
      },
      stopInerval(){
        clearInterval(this.makeActive)
      }
    },
    mounted(){
      this.intervalId1 = setInterval(this.makeActive, 3000)
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

#mygallery{
  .active_img_slider{
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: 1;
    filter:brightness(0.5);
  }
  .container{
    z-index: 2;
    min-height: 500px;
  }
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

  .active_slider_button{
    transform: translateY(-10px);
    transition: 0.3s;
  }
  
}
 
 
</style>
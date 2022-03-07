<template>
  <section id="overview" >
      <div class="container px-5 py-5">
        <div class="row mx-5">
          <div class="col-5 d-flex flex-column">

            <div class="btn-box">
            <button class="ms_btn_primary ms_w-min">
              overview
            </button>
            <button class="ms_btn_primary ms_w-min text-nowrap mx-1">
              Our Mission
            </button>
            </div>

            <p class="fs-3 mt-4 lh-sm seco">
              Our philosophy is learning through play as we offer a stimulating environment for children.
            </p>

 
            <div v-for="(badgeBox, index) in badgeBoxes" :key="index" class="badge-box-hor">
              <div class="badge-icon-primary">
                <img :src="badgeBox.url" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title fs-4 fw-light">{{badgeBox.title}}</h4>
                <p class="badge-caption fs-6 text-secondary fw-light">{{badgeBox.text}}</p>
              </div>
            </div>


          </div>
          <div class="col ">
              <div class="current-img mb-3 position-relative">
                <i @click="nextPic" class="fa-solid fa-chevron-right position-absolute top-50 end-0 p-2  fs-5 bg-prim text-white"></i>
                <i @click="previousPic" class="fa-solid fa-chevron-left  position-absolute top-50  p-2  fs-5  bg-prim text-white"></i>
                <img class="img-fluid" :src="currentImages[active].url" alt="">
              </div>
              <div class="row g-3">
                <div v-for="(currentImage,index) in currentImages" :key="index" class="col">
                  <img class="ms_thumbnail" :class="[index == active ? 'ms_active' : '']" :src="currentImages[index].url" alt="">
                </div>
              </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>

export default {
    name: "MyOverview",
    data(){
      return{
        badgeBoxes : [
          {
            title: "Full Day Sessions",
            text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione!",
            url: "../badge-box-hor-icons/clock_alt.png"
          },
          {
            title: "Varied Classes",
            text: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione!",
            url: "../badge-box-hor-icons/diagram_alt.png"

          },
        ],
        currentImages: [
          {
            url: "../slider_big-images/gallery_07-690x506.jpg"
          },
          {
            url: "../slider_big-images/gallery_01-690x506.jpg"
          },
          {
            url: "../slider_big-images/gallery_08-690x506.jpg"
          },
        ],

        active : 0
      }
    },
    methods: {
      nextPic(){
        if(this.active < this.currentImages.length - 1){
          this.active++
        }else{
          this.active = 0
        }
      },
      previousPic(){
        if(this.active > 0){
          this.active--
        }else{
          this.active = this.currentImages.length - 1
        }
      },
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';
#overview{
  background-color: $customGrey;
}



//TODO FINIRE SLIDER


// Slider 
.ms_thumbnail{
width: 100%;
object-fit: contain;
}
 
// effetto per dare alle thumbanils l'effetto di selezionato 
.ms_active{
    border-bottom: 2px solid red;
    padding-bottom: 1rem;
}

</style>
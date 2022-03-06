<template>
  <section id="whatsnew" class="d-flex align-items-center py-5">
    <div class="container py-2">
          <div class="row ">
        <div class="col text-center">
        <h2 class="seco fw-light">Welcome to Fable</h2>
            <p class="text-secondary fw-light">Family daycare, preschool, and kindergarten</p>
            <p class="orbitron">/\/\/\/</p>

        </div>
      </div>
      <div class="row  row">
        <div class="col-4 p-3">
          <MyCardVert/>
        </div>
        <div class="col-4 p-3">
          <MyCardVert/>
        </div>
        <div class="col-4 p-3">
          <MyCardVert/>
        </div>
        <div class="col-12 text-center">
          <button class="ms_btn_primary my-3">
            GO TO BLOG 
            <i class="fa-solid fa-chevron-right ms-2"></i>
          </button>
        </div>
      </div>
      
    </div>

 
  </section>
</template>

<script>
import MyCardVert from './partials/MyCardVert.vue'

export default {
    name: "MyWhatsNew",
    components:{
      MyCardVert
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';


 
 
</style>
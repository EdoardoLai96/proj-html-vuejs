<template>
  <section id="whatsnew" class="d-flex align-items-center debug-container">
    <div class="container">
          <div class="row debug-row">
        <div class="col debug-col text-center">
        <h2>Welcome to Fable</h2>
            <p>Family daycare, preschool, and kindergarten</p>
            <p>/\/\/\/</p>

        </div>
      </div>
      <div class="row debug row">
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
            GO TO BLOG >
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
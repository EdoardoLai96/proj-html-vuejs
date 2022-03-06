<template>
  <section id="whatsnew" class="d-flex align-items-center py-5">
    <div class="container py-2">
          <div class="row ">
        <div class="col text-center">
        <h2 class="seco fw-lighter fs-1">What's New</h2>
            <p class="text-secondary fw-light">Family daycare, preschool, and kindergarten</p>
            <p class="orbitron">/\/\/\/</p>

        </div>
      </div>
      <div class="row  row">
        <div v-for="(cardVert, index) in cardsVert" :key="index" class="col-4 p-3">
          <MyCardVert :cardVert="cardsVert[index]"/>
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
    },
    data(){
      return{
        cardsVert: [
          {
            date: "October 03, 2014",
            title: "Drawing and Painting Lessons",
            text: "Lorem ipsum dolor sit amet, consectetur adipisci elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam",
            size: "42",
            author: "Anna Brown",
            category:"Events, Fun",
            url: "../card-vert-images/card-vert_01.jpg"
          },
          {
            date: "November 5, 2014",
            title: "Fall Parents Meeting Day",
            text: "Lorem ipsum dolor sit amet, consectetur adipisci elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam",
            size: "19",
            author: "Anna Brown",
            category:"Dance, Education",
            url: "../card-vert-images/card-vert_02.jpg"

          },
          {
            date: "September 4, 2014",
            title: "Birthday in Kindergarten",
            text: "Lorem ipsum dolor sit amet, consectetur adipisci elit, sed eiusmod tempor incidunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam",
            size: "22",
            author: "Anna Brown",
            category:"Games, General",
            url: "../card-vert-images/card-vert_03.jpg"
          },
        ]
      }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';


 
 
</style>
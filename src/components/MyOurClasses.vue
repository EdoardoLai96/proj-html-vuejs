<template>
  <section id="ourclasses" class="p-5">
    <div class="container">
      <div class="row mx-5">
        <div class="col  text-center">
        <h2 class="seco fw-light">Our Classes</h2>
            <p class="text-secondary">Our preschool program has four dedicated classes</p>
            <p class="orbitron mb-5">/\/\/\/</p>
        </div>
      </div>

      <div class="row mx-5">
        <div class="col ">
          <p class="seco fs-4 pb-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rerum voluptas, odio debitis sit inventore voluptate delectus nobis, odit.</p>
        </div>
        <div class="col ">
          <p class="text-secondary pt-2 right-par">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed molestiae, quod saepe tempora odit placeat voluptatem corporis accusantium cum velit dolores veritatis, est debitis in magnam beatae! Quod, similique amet.
          </p>
        </div>
      </div>

      <div class="row mx-5  g-4 pb-2">

         <div v-for="(cardHor, index) in cardsHor" :key="index" class="col-6">
           <MyCardHor :cardHor="cardsHor[index]"/>
         </div>

      </div>
    </div>
  </section>
</template>

<script>
import MyCardHor from '../components/partials/MyCardHor.vue'

export default {
    name: "MyOurClasses",
    components: {
      MyCardHor
    },
    data(){
      return{
        cardsHor: [
          {
            title: "Little Lambs",
            name: "Class Name",
            age_range: "12-24",
            age_class: "Month Olds",
            size: 9,
            url: "../../card-hor-images/card-hor_01.jpg"
          },
          {
            title: "Bouncy Bears",
            name: "Class Name",
            age_range: "2-3",
            age_class: "Year Olds",
            size: 12,
            url: "../../card-hor-images/card-hor_02.jpg"

          },
          {
            title: "Tender Hearts",
            name: "Class Name",
            age_range: "3-4",
            age_class: "Year Olds",
            size: 15,
            url: "../../card-hor-images/card-hor_03.jpg"
          },
          {
            title: "Shining Stars",
            name: "Class Name",
            age_range: "4-5",
            age_class: "Year Olds",
            size: 20,
            url: "../../card-hor-images/card-hor_04.jpg"
          },
        ]
      }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';


.right-par{
  font-size: 0.9rem;
}

 
</style>
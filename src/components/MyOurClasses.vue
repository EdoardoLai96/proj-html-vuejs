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

         <div class="col-6">
           <MyCardHor/>
         </div>

         <div class="col-6">
           <MyCardHor/>
          </div>

         <div class="col-6">
           <MyCardHor/>
         </div>

         <div class="col-6">
           <MyCardHor/>
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
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';


.right-par{
  font-size: 0.9rem;
}

 
</style>
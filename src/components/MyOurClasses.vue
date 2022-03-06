<template>
  <section id="ourclasses">
    <div class="container ">
      <div class="row ">
        <div class="col  text-center">
        <h2>Welcome to Fable</h2>
            <p>Family daycare, preschool, and kindergarten</p>
            <p>/\/\/\/</p>
        </div>
      </div>

      <div class="row ">
        <div class="col ">
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Rerum voluptas, odio debitis sit inventore voluptate delectus nobis, odit, pariatur quisquam sint quo! Et eius numquam tempore eligendi! Voluptas, explicabo? Rem.</p>
        </div>

        <div class="col ">
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed molestiae, quod saepe tempora odit placeat voluptatem corporis accusantium cum velit dolores veritatis, est debitis in magnam beatae! Quod, similique amet.
          </p>
        </div>
      </div>

      <div class="row  gx-4 gy-4">

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




/// .debug-card{
//   height: 200px;
//   border: 1px solid black;
// }
 
</style>
<template>
  <section id="mygoals">
    <div class="container p-5">

      <div class="row mx-4">
        <div class="col-6">
          <p class="seco fs-4 lh-sm">We have been educating children for over fifteen yars. Our goal is to create a place that engages each child.</p>
          <p class="text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae cumque excepturi facilis qui nam necessitatibus. Eligendi perspiciatis eos dolorem, est, voluptatum autem officiis.</p>
          <div class="checbox-box">
            <div v-for="(goal, index) in goals" :key="index" class="checkbox-box_item mb-2">
              <img class="me-3" src="../assets/images/style_1.png" alt="">
              <span class="text-secondary">{{goal}}</span>
            </div>
          </div>
        </div>
        <div class="col-6">
          <div class="row">
            <div v-for="(badgeBoxSmall, index) in badgeBoxesSmall" :key="index" class="col-6 p-0">
              <MyBadgeBoxSmall :badgeBoxSmall="badgeBoxesSmall[index]"/>

            </div>


          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid">

      <div class="row">
        <div class="col-3 p-0">
          <img src="" class="w-100" alt="">
        </div>
        <div class="col-3 p-0">
          <img src="" class="w-100" alt="">
        </div>
        <div class="col-3 p-0">
          <img src="" class="w-100" alt="">
        </div>
        <div class="col-3 p-0">
          <img src="" class="w-100" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import MyBadgeBoxSmall from "../components/partials/MyBadgeBoxSmall.vue"

export default {
    name: "MyGoals",
    components: {
      MyBadgeBoxSmall
    },
    data(){
      return{
        badgeBoxesSmall : [
        {
          title: "Learning & Fun",
          text: "Custom medium lenght text 1 averagely long the first of 4 cards.",
          background: "prim",
          url: "../badge-box-vert-small-icons_goals/toy.png"
        },
        {
          title: "Healthy Meals",
          text: "Custom medium lenght text 2 averagely long, second of 4 cards.",
          background: "seco",
          url: "../badge-box-vert-small-icons_goals/meal.png"
        },
        {
          title: "Friendly Place",
          text: "Custom medium lenght text 3 averagely long the third of 4 cards.",
          background: "prim",
          url: "../badge-box-vert-small-icons_goals/school.png"
        },
        {
          title: "Children Safety",
          text: "Custom medium lenght text 4 averagely long the fourth of 4 cards.",
          background: "seco",
          url: "../badge-box-vert-small-icons_goals/shield.png"
        },
        ],

        // Elenco dei goal, è possibile aggiungerne o rimuoverne direttamente da questa lista e verranno stampati dinamicamente a schermo

        goals : [
          "Comprehensive reporting on individual achievement",
          "Educational field trips and school presentations",
          "Individual attention in a small-class setting",
          "Learning program with after school care",
          "Opportunities to carry out scientific investigations",
          "Positive learning environement for your child",
        ]
      }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

#mygoals{
  background-color: $customGrey;
}

.debug-col{
  border: 2px solid white;
}
 
 
</style>
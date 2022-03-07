<template>
  <section id="welcome">
      <div class="container py-4 px-5">
        <div class="row">
          <div class="col debug text-center">
            <h2 class="fs-1 fw-lighter">Welcome to Fable</h2>
            <p class="text-secondary fw-light">Family daycare, preschool, and kindergarten</p>
            <p class="orbitron">/\/\/\/\/</p>

          </div>
        </div>
        <div class="row">

          <div v-for="(badgeBox, index) in badgeBoxes" :key="index" class="col debug d-flex justify-content-center">
            <MyBadgeBox :badgeBox="badgeBoxes[index]" />
          </div>

        </div>
      </div>
  </section>
</template>

<script>
import MyBadgeBox from "../components/partials/MyBadgeBox.vue"

export default {
    name: "MyWelcome",
    components: {
      MyBadgeBox
    },
    data(){
      return{
        // ARRAY CONTENENTE TUTTI I BADGE BOXES E LE LORO PROPRIETA', PER AGGIUNGERNE O TOGLIERNE DA QUESTA SEZIONE BASTA AGIRE SU QUESTA LISTA
        badgeBoxes: [
        {
          title: "Morbi Etos",
          text: "Custom long text 1 very very very very long  the first of 4 cards, really long text used as a filler to fill the paragraph of the card",
          background: "prim",
          url: "../../badge-box-vert-icons/schoolbag_alt.png"
        },
        {
          title: "Congue Gravida",
          text: "Custom long text 2 very very very very long  the second of 4 cards, really long text used as a filler to fill the paragraph of the card",
          background: "seco",
          url: "../../badge-box-vert-icons/stroller_alt.png"
        },
        {
          title: "Maecenas Node",
          text: "Custom long text 3 very very very very long  the third of 4 cards, really long text used as a filler to fill the paragraph of the card",
          background: "prim",
          url: "../../badge-box-vert-icons/globe_alt.png"
        },
        {
          title: "Praesent Morbi",
          text: "Custom long text 4 very very very very long  the fourth of 4 cards, really long text used as a filler to fill the paragraph of the card",
          background: "seco",
          url: "../../badge-box-vert-icons/bell_alt.png"
        },
          ]

      }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

 
 
h2{
  color: $secondaryColor;
}
 
</style>
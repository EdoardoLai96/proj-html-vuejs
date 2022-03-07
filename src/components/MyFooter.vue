<template>
  <footer id="contactus">
    <div class="container py-5">
      <div class="row">
        <div class="col text-center">
        <h2 class="seco fw-light">Welcome to Fable</h2>
            <p class="text-secondary fw-light">Family daycare, preschool, and kindergarten</p>
            <p class="orbitron">/\/\/\/</p>
        </div>
      </div>
      <div class="row justify-content-center">

          <div v-for="(badgeBoxSmall, index) in badgeBoxesSmall" :key="index" class="col-2  d-flex justify-content-center">
            <MyBadgeBoxSmall :badgeBoxSmall="badgeBoxesSmall[index]"/>
          </div>

      </div>
      <div class="row">
        <div class="col">
          <div class="form-container-left">
            <input type="text" class="mb-3 w-100 p-2 fs-7" id="name_form" placeholder="Your Name*">
            <input type="email" class="mb-3 w-100 p-2 fs-7" id="email_form" placeholder="Your E-mail*">
            <input type="text" class=" w-100 p-2 fs-7" id="subject_form" placeholder="Subject">
          </div>
        </div>
        <div class="col">
          <div class="form-container-right">

            <textarea class="w-100 p-2 ms_text_area" id="msg_form" rows="6" placeholder="Your Messsage *"></textarea>
            <!-- <textarea class="form-control ms_text_area" id="exampleFormControlTextarea1" rows="6"></textarea> -->
          </div>

        </div>
      </div>

    </div>
  </footer>
</template>

<script>
import MyBadgeBoxSmall from '../components/partials/MyBadgeBoxSmall.vue'

export default {
    name: "MyFooter",
    components: {
      MyBadgeBoxSmall
    },
    data(){
      return{
        badgeBoxesSmall : [
          {
            title: "Postal Address",
            text: " Fable Care Center 85 Fentiman Ave, <br/> Ottawa ON and K1S 0T7 ",
            background: null,
            url: "../badge-box-vert-small-icons_footer/envelope_primary.png"
          },
          {
            title: "Phone & Email",
            text: "Phone: 1-800-64-38 Fax: 1-800-64-39 office@fable.com",
            background: null,
            url: "../badge-box-vert-small-icons_footer/mobile.png"
          },
          {
            title: "Business Hours",
            text: "Monday - Friday 8.00 am - 5.00 pm Weekend Closed",
            background: null,
            url: "../badge-box-vert-small-icons_footer/clock.png"
          },
          {
            title: "Sessions",
            text:"Mornings, 8 am - 12 pm <br/> Afternoons, 1 pm - 5 pm Full Day, 8 am - 5 pm",
            background: null,
            url: "../badge-box-vert-small-icons_footer/document_prim.png"
          },
        ],

      }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

.form-container-left{
  input{
  height: calc((165px - 2rem) / 3);
  outline: none;
  border: 1px solid rgb(196, 196, 196);
  }
}

.ms_text_area{
  height: 165px;
  outline: none;
}

.form-container-right{
  height: 200px;
  textarea{
  border: 1px solid rgb(196, 196, 196);

  }
  
}
 
 
</style>
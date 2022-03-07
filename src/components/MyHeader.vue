<template>


  <header class="">
    <div  class="container  px-5 align-items-center">
      <div class="row  justify-content-between"> 

        <!-- PARTE HEADER DI SINISTRA CON LOGO  -->

        <div class="col-5 d-flex align-items-center justify-content-center">
          <div class="img-box d-flex">
          <img src="../assets/images/logo_cropped.png" alt="">
          </div>
        </div>

        <!-- PARTE HEADER DI SINISTRA CON NAV  -->

        <nav class="col-7 d-flex justify-content-center">
        <!-- ELEMENTI INSERITI DINAMICAMENTE DA DATA TRAMITE CICLO FOR  -->

        <MyNavItem v-for="(nav_item, index) in nav_items" :key="index"  :nav_item="nav_items[index]"/>

        </nav>

      </div>
    </div>
  </header>
</template>

<script>
import MyNavItem from '../components/partials/MyNavItem.vue'
export default {
    name: "MyHeader",
    components: {
      MyNavItem
    },

    data(){
      return{

        // ARRAY CHE CONTIENE TUTTI I NAV ITEMS, SE SI VUOLE AGGIUNGERE UNA VOCE AL MENU' BASTA AGGIUNGERE IL DATO QUA SOTTOFORMA DI OGGETTO E AUTOMATICAMENTE SI POPOLERA' 
        nav_items : [
          {
            href: "#jumbotron",
            text: "Home",
            icon_name: "fa-solid fa-house"
          },
          {
            href: "#welcome",
            text: "Pages",
            icon_name: "fa-solid fa-file-lines"
          },
          {
            href: "#overview",
            text: "Blog",
            icon_name: "fa-solid fa-print"
          },
          {
            href: "#ourclasses",
            text: "Shop",
            icon_name: "fa-solid fa-cart-arrow-down"
          },
          {
            href: "#mygoals",
            text: "Shortcodes",
            icon_name: "fa-solid fa-flask"
          },
          {
            href: "#contactus",
            text: "Support",
            icon_name: "fa-solid fa-headset"
          },
          {
            href: "#contactus",
            text: "Contact",
            icon_name: "fa-solid fa-envelope"
          },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
 @import "../assets/style/variables.scss";

header{
  .img-box{
    text-align: center;
      img{
      width: 120px;
      height: auto;
    }
  }
  .nav-item{
    text-decoration: none;
    &:hover{
      background-color: $primaryColor;
      color: white;
      cursor: pointer;
      transition: background-color 0.4s;
    }
    .nav_icon{
      transform: scale(0.8);
    }
  }
}






//
 
</style>
<template>
  <section id="welcome" class="debug-container">
      <div class="container py-4 px-5">
        <div class="row">
          <div class="col debug-col text-center">
            <h2>Welcome to Fable</h2>
            <p>Family daycare, preschool, and kindergarten</p>
            <p>/\/\/\/</p>

          </div>
        </div>
        <div class="row">

          <div class="col debug-col d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon prim">
                <img src="../assets/images/stroller_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

          <div class="col debug-col d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon sec">
                <img src="../assets/images/stroller_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

          <div class="col debug-col d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon prim">
                <img src="../assets/images/stroller_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

          <div class="col debug-col d-flex justify-content-center">
            <div class="badge-box-ver prim">
              <div class="badge-icon sec">
                <img src="../assets/images/stroller_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

       

        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "MyWelcome"

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

.badge-icon.prim{
  background-color: $primaryColor;
}
 
.badge-icon.sec{
  background-color: $secondaryColor;
}
 
 
</style>
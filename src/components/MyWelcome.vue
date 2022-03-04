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

          <div class="col debug d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon prim">
                <img src="../assets/images/schoolbag_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title  my-3">Badge Title</h4>
                <p class="badge-caption text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

          <div class="col debug d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon sec">
                <img src="../assets/images/stroller_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title  my-3">Badge Title</h4>
                <p class="badge-caption text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

          <div class="col debug d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon prim">
                <img src="../assets/images/globe_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title  my-3">Badge Title</h4>
                <p class="badge-caption text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

          <div class="col debug d-flex justify-content-center">
            <div class="badge-box-ver prim">
              <div class="badge-icon sec">
                <img src="../assets/images/bell_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title  my-3">Badge Title</h4>
                <p class="badge-caption text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
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
 
h2{
  color: $secondaryColor;
}
 
</style>
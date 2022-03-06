<template>
  <section id="overview" >
      <div class="container px-5 py-5">
        <div class="row">
          <div class="col-5 d-flex flex-column">

            <div class="btn-box">
            <button class="ms_btn_primary ms_w-min">
              overview
            </button>
            <button class="ms_btn_primary ms_w-min text-nowrap mx-1">
              Our Mission
            </button>
            </div>

            <p class="fs-5 mt-4">
              Our philosophy is learning through play as we offer a stimulating environment for children.
            </p>


            <div class="badge-box-hor">
              <div class="badge-icon-primary">
                <img src="../assets/images/clock_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione!</p>
              </div>
            </div>

            <div class="badge-box-hor">
              <div class="badge-icon-primary">
                <img src="../assets/images/diagram_alt.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption text-secondary">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione!</p>
              </div>
            </div>


          </div>
          <div class="col ">
              <div class="current-img mb-3 position-relative">
                <i class="fa-solid fa-chevron-right position-absolute top-50 end-0 p-2  fs-5 "></i>
                <i class="fa-solid fa-chevron-left  position-absolute top-50  p-2  fs-5 "></i>
                <img class="img-fluid" src="../assets/images/gallery_08-690x506.jpg" alt="">
              </div>
              <div class="row g-3">
                <div class="col">
                  <img class="ms_thumbnail ms_active" src="../assets/images/gallery_07-690x506.jpg" alt="">
                </div>
                <div class="col">
                  <img class="ms_thumbnail" src="../assets/images/gallery_01-690x506.jpg" alt="">
                </div>
                <div class="col" >
                  <img class="ms_thumbnail" src="../assets/images/gallery_08-690x506.jpg" alt="">

                </div>
              </div>
          </div>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "MyOverview"

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';
#overview{
  background-color: $customGrey;
}



//TODO FINIRE SLIDER


// Slider 
.ms_thumbnail{
width: 100%;
object-fit: contain;
}
 
// effetto per dare alle thumbanils l'effetto di selezionato 
.ms_active{
    border-bottom: 2px solid red;
    padding-bottom: 1rem;
}

// posizionamento e stile delle freccette per scorrere le immagini
.current-img{
  i{
    color: white;
    background-color: $primaryColor;
  }
}

</style>
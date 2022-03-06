<template>
        <!-- Card orizzontale, usata solo nella sezione "OurClasses" lo stile e scoped e valido solo in questo componente -->
    <div class="ms_card justify-content-between d-flex bg-seco text-white">
        <div class="ms_card__text-box  d-flex flex-column justify-content-between p-3">
            <div class="ms_card__text-box-top">
                <h2 class="ms_card_title fs-4 mb-0">{{cardHor.title}}</h2>
                <p class="fw-light">{{cardHor.name}}</p>
            </div>
            <div class="ms_card__text-box-bottom">
                <div class="ms_card__text-box-bottom_left my-1 w-50 d-inline-block text-center border-end">
                    <h4 class="my-0 ms_card_age fs-6"> {{cardHor.age_range}} </h4>
                    <p class="my-0"> {{cardHor.age_class}}</p>
                </div>
                <div class="ms_card__text-box-bottom_lright my-1 w-50 d-inline-block text-center">
                    <h4 class="my-0 ms_card_size fs-6">{{cardHor.size}}</h4>
                    <p class="my-0">Class Size</p>
                </div>
            </div>
        </div>
        <div class="img-box  position-relative">
            <img class="w-100 h-100 ms_fit_cover" :src="cardHor.url" alt="">
            <button class="ms_btn_primary position-absolute bottom-0 end-0">
               READ MORE 
               <i class="ms-1 fa-solid fa-chevron-right"></i>
            </button>
        </div>
    </div>
</template>

<script>
export default {
name: "MyCardHor",
props: {
    cardHor: Object
}
}
</script>

<style lang="scss" scoped>
.ms_card{
  height: 200px;
  .ms_card__text-box{
      flex-basis: 50%;
  }
}

</style>
<template>
  <div class="cta px-5 py-2 bg-seco">
      <div class="container px-5 py-3">
        <div class="row mx-5">
            <div class="col-7">
                <h3 class="fs-4">{{cta.text}}</h3>
            </div>
            <div class="col-5 text-center justify-content-center">
                <button class="ms_btn_secondary">
                    {{cta.button}} 
                    <i class="fa-solid fa-chevron-right ms-2"></i>
                </button>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyCallToAction",
    props: {
      cta : Object
    }

}
</script>

<style lang="scss" scoped>
 @import '../../assets/style/variables.scss';

  .cta{
      color: white;
      h3{
        margin-bottom: 0;
        font-weight: lighter;
      }
  }  

 //Debug// 

.debug-col{
  background-color: #1bafe4;
  margin: 1px;
  
  }
.debug-row{
  background-color: #fcd902;
  
}
.debug-container{
  background-color: #d71938;
}
 

 
</style>
<template>
  <div class="cta py-2">
      <div class="container px-5 py-3">
        <div class="row">
            <div class="col-7">
                <h3 class="fs-4">How To Enroll Your Child to a Class?</h3>
            </div>
            <div class="col-5 text-center justify-content-center">
                <button class="ms_btn_secondary">
                    LEARN MORE >
                </button>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyCallToAction"

}
</script>

<style lang="scss" scoped>
 @import '../../assets/style/variables.scss';

  .cta{
      background-color: $secondaryColor;
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
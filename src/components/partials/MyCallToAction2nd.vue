<template>
  <div class="cta">
      <div class="container px-5 py-3">
        <div class="row">
            <div class="col-7">
                <h3>See Our Kindergarten Photo Gallery!</h3>
            </div>
            <div class="col-5 text-center justify-content-center">
                <button class="ms_btn_secondary">
                    VIEW GALLERY >
                </button>
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name: "MyCallToAction2nd"

}
</script>

<style lang="scss" scoped>
 @import '../../assets/style/variables.scss';

  .cta{
      background-image: url('../../assets/images/pattern.png');
      background-size: cover;
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
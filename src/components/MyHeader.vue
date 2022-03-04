<template>
  <header class="">
    <div  class="container  px-5 align-items-center">
      <div class="row  justify-content-between"> 
        <div class="col-5 d-flex align-items-center justify-content-center">
          <div class="img-box d-flex">
          <img src="../assets/images/logo_cropped.png" alt="">
          </div>
        </div>

        <div class="col-7 d-flex justify-content-center">
        <a href="#jumbotron" class=" nav-item  mx-2 py-2 px-3 text-center">
          <i class="fs-4 fa-solid fa-house"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        <a href="#welcome" class=" nav-item  mx-2 py-2 px-3 text-center">
          <i class="fs-4 fa-solid fa-file-lines"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        <a href="#overview" class=" nav-item  mx-2 py-2 px-3 text-center">
          <i class="fs-4 fa-solid fa-print"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        <a href="#ourclasses" class=" nav-item  mx-2 py-2 px-3 text-center">
          <i class="fs-4 fa-solid fa-cart-arrow-down"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        <a href="#mygoals" class=" nav-item  mx-2 py-2 px-3 text-center">
         <i class="fs-4 fa-solid fa-flask"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        <a href="#contactus" class=" nav-item  mx-2 py-2 px-3 text-center">
          <i class="fs-4 fa-solid fa-headset"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        <a href="#contactus" class=" nav-item  mx-2 py-2 px-3 text-center">
          <i class="fs-4 fa-regular fa-envelope"></i>
          <p class="text-center mb-0">Text</p>
        </a>
        </div>

      </div>
    </div>
  </header>
</template>

<script>
export default {
    name: "MyHeader"

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
    color: $secondaryColor;
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
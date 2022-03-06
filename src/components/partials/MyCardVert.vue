<template>
  <div class="MyCardVert">
      <span class="text-secondary d-block">Date</span>
      <div class="img-box w-100 h-100 position-relative my-4">
          <img class="w-100" src="../../assets/images/blog_09-300x180.jpg" alt="">
          <div class="partecipants position-absolute bottom-0 end-0">
              42
          </div>
      </div>
        <h4 class="seco fs-4 fw-light">Card Title</h4>
        <p class="text-secondary fs-6">Card Caption</p>
        <hr class="my-1 text-secondary">
        <div class="card_footer"> 
            <img class="me-3 " src="../../assets/images/author.png" alt="">
            <span class="align-middle text-secondary">Author</span>
            <img class="me-3 ms-3" src="../../assets/images/category.png" alt="">
            <span class="align-middle text-secondary">Category</span>
        </div>
  </div>
</template>

<script>
export default {

name: "MyCardVert"
}
</script>

<style lang="scss" scoped>
 @import '../../assets/style/variables.scss';

.partecipants{
    background-color: $primaryColor;
    padding: 0.2rem 0.4rem ;
    color: white;
}

.card_footer span{
    display: inline-block;
    font-size: 0.75rem;
}



</style>
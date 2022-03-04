<template>
  <footer id="contactus">
    <div class="container">
      <div class="row">
        <div class="col text-center">
        <h2>Welcome to Fable</h2>
            <p>Family daycare, preschool, and kindergarten</p>
            <p>/\/\/\/</p>
        </div>
      </div>
      <div class="row">

          <div class="col-3 d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon p-0">
                <img src="../assets/images/envelope_primary.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>
          <div class="col-3 d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon p-0 ">
                <img src="../assets/images/mobile.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>
          <div class="col-3 d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon p-0 ">
                <img src="../assets/images/clock.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>
          <div class="col-3 d-flex justify-content-center">
            <div class="badge-box-ver">
              <div class="badge-icon p-0 ">
                <img src="../assets/images/document_prim.png" alt="">
              </div>
              <div class="badge-text">
                <h4 class="badge-title">Badge Title</h4>
                <p class="badge-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Eveniet, ratione! Perferendis inventore nam aliquid minima pariatur </p>
              </div>
            </div>
          </div>

      </div>
      <div class="row">
        <div class="col">
          <div class="form-container-left">
            <input type="text" class="mb-3 w-100 p-2 fs-7" id="name_form" placeholder="Your Name*">
            <input type="email" class="mb-3 w-100 p-2 fs-7" id="email_form" placeholder="Your E-mail*">
            <input type="text" class=" w-100 p-2 fs-7" id="subject_form" placeholder="Subject">
          </div>
        </div>
        <div class="col">
          <div class="form-container-right">

            <textarea class="w-100 p-2 ms_text_area" id="msg_form" rows="6" placeholder="Your Messsage *"></textarea>
            <!-- <textarea class="form-control ms_text_area" id="exampleFormControlTextarea1" rows="6"></textarea> -->
          </div>

        </div>
      </div>

    </div>
  </footer>
</template>

<script>
export default {
    name: "MyFooter"

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

.form-container-left{
  input{
    height: calc((165px - 2rem) / 3);
  outline: none;
  }
}

.ms_text_area{
  height: 165px;
  outline: none;
}

.form-container-right{
  height: 200px;
}
 
 
</style>
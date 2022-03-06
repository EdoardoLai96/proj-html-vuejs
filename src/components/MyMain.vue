<template>
  <main>
      <MyJumbotron/>
      <MyCallToAction :cta="ctas[0]"/>
      <MyWelcome/>
      <MyOverview/>
      <MyOurClasses/>
      <MyGoals/>
      <section class="cta_bg-custom">
        <MyCallToAction :cta="ctas[1]"/>
      </section>
      <MyGallery/>
      <MyWhatsNew/>
      <MyMap/>
  </main>
</template>

<script>
import MyJumbotron from '../components/MyJumbotron'
import MyCallToAction from '../components/partials/MyCallToAction'
import MyWelcome from '../components/MyWelcome'
import MyOverview from '../components/MyOverview'
import MyOurClasses from '../components/MyOurClasses'
import MyGoals from '../components/MyGoals'
import MyWhatsNew from '../components/MyWhatsNew'
import MyGallery from '../components/MyGallery'
import MyMap from '../components/MyMap'


export default {
    name: "MyMain",
    components:{
        MyJumbotron,
        MyCallToAction,
        MyWelcome,
        MyOverview,
        MyOurClasses,
        MyGoals,
        MyWhatsNew,
        MyGallery,
        MyMap
    },
    data(){
        return{
            ctas : [
                {   
                    text: "How to Enroll Your Child to a Class?",
                    button: "LEARN MORE",
                    bg_custom: false
                },
                {   
                    text: "See Our Kindergarten Photo Gallery!",
                    button: "VIEW GALLERY",
                    bg_custom: true
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';


// custom bg per cta
.cta_bg-custom{
    background-image: url('../assets/images/pattern.png');
    background-size: cover;
    background-position: center;
}
 
 
</style> 
<template>
  <main>
      <MyJumbotron/>
      <MyCallToAction :cta="ctas[0]"/>
      <MyWelcome/>
      <MyOverview/>
      <MyOurClasses/>
      <MyGoals/>
      <MyCallToAction2nd/>
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
import MyCallToAction2nd from '../components/partials/MyCallToAction2nd'
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
        MyCallToAction2nd,
        MyWhatsNew,
        MyGallery,
        MyMap
    },
    data(){
        return{
            ctas : [
                {   
                    text: "How to Enroll Your Child to a Class?",
                    button: "LEARN MORE"
                },
                {   
                    text: "See Our Kindergarten Photo Gallery!",
                    button: "VIEW GALLERY"
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

 
 
</style> 
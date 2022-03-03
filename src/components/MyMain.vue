<template>
  <div>
      <MyJumbotron/>
      <MyCallToAction/>
      <MyWelcome/>
      <MyOverview/>
      <MyOurClasses/>
      <MyGoals/>
      <MyWhatsNew/>
      <MyMap/>
  </div>
</template>

<script>
import MyJumbotron from '../components/MyJumbotron'
import MyCallToAction from '../components/partials/MyCallToAction'
import MyWelcome from '../components/MyWelcome'
import MyOverview from '../components/MyOverview'
import MyOurClasses from '../components/MyOurClasses'
import MyGoals from '../components/MyGoals'
import MyWhatsNew from '../components/MyWhatsNew'
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
        MyMap
    }

}
</script>

<style lang="scss" scoped>
 @import '../assets/style/variables.scss';

 
 
</style> 
<template>
  <div>
      <MyJumbotron/>
      <MyOverview/>
      <MyOurClasses/>
      <MyGoals/>
      <MyWhatsNew/>
      <MyMap/>
  </div>
</template>

<script>
import MyJumbotron from '../components/MyJumbotron'
import MyOverview from '../components/MyOverview'
import MyOurClasses from '../components/MyOurClasses'
import MyGoals from '../components/MyGoals'
import MyWhatsNew from '../components/MyWhatsNew'
import MyMap from '../components/MyMap'


export default {
    name: "MyMain",
    components:{
        MyJumbotron,
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
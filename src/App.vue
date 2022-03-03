<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>

  </div>
</template>

<script>
import MyHeader from './components/MyHeader'
import MyMain from './components/MyMain'
import MyFooter from './components/MyMain'


export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
  }
}
</script>

<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style/variables.scss';
  #app{
    background-color: white;
  }
</style>

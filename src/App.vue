<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <shopperContent>
    <MyFooter/>
    

    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyMain from './components/MyMain';
import shopperContent from './components/shopperContent.vue';
import MyFooter from './components/MyFooter';
import ShopperContent from './components/shopperContent.vue';


export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
    ShopperContent
}
}
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap.scss';
@import './styles/general.scss';
@import './styles/variables.scss'


</style>

<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
    

    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyMain from './components/MyMain';
import MyFooter from './components/MyFooter';


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
@import '~bootstrap/scss/bootstrap.scss';
@import './styles/general.scss';
@import './styles/variables.scss'


</style>

<template>
  <div id="app">
    <Header/>
    <Banner/>
    <MainTop/>
    <MainBottom/>
    <FooterTop/>
    <FooterBottom/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Banner from './components/Banner.vue'
import MainTop from './components/MainTop.vue'
import MainBottom from './components/MainBottom.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'



export default {
  
  name: 'App',
  components: {
    Header,
    Banner,
    MainTop,
    FooterTop,
    FooterBottom,
    MainBottom,
  }
  
}
</script>

<style lang="scss">
@import "./components/style/Common";

</style>

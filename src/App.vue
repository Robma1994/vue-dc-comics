<template>
  <div id="app">
    <Header/>
    <MainTop/>
    <FooterTop/>
    <FooterBottom/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import MainTop from './components/MainTop.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainTop,
    FooterTop,
    FooterBottom
  }
}
</script>

<style lang="scss">
@import "./components/style/Common";

</style>

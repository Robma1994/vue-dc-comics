<template>
  <div class="container-large">
    <div class="container-small">
        <img :src="cart.thumb" alt="">
        <h2>{{cart.series}}</h2>
    </div>
  </div>
</template>

<script>

export default {
  name: 'MainFumetti',
  props: ['cart']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 

</style>

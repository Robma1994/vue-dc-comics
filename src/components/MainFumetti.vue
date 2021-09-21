<template>
  <div>
    <div class="containerImg">
      <img :src="cart.thumb">
      <div>
        <h2 class="title">{{cart.series}}</h2> 
      </div>
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
.containerImg {
  width: 180px;
  padding: 10px;
    img {
      width: 100%;
    }
}
.title {
  font-size: 20px;
}
</style>

<template>
  <div class="container-large">
    <div class="container-small">
      <h1 class="title"> Content goes here </h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainTop',
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/Variables";
.container-large {
  background-color: black;
}
.container-small {
  padding: 40px 0 40px 0;
  background-color: black;
}
.title{
  color: $colorTitle;
  font-size: $fontSizeTitle;

  &::before {
    content: '-->';
  }
  &::after {
    content: '<--';
  }
}
</style>

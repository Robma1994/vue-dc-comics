<template>
  <div class="container-large">
    <div class="container-small">
      <div class="btn-left">
        <button>SIGN-UP NOW</button>
      </div>
      <div class="social-right">
        <h2>FOLLOW US</h2>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'FooterBottom',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/Variables";
.container-large {
  height: 120px;
  background-color: $backgroundColorFooter;
  .container-small {
    height: 100%;
    display: flex;
    justify-content: space-between;
    .btn-left, .social-right {
      display: flex;
      align-items: center;

      button {
        width: 110px;
        height: 50px;
        background-color: $backgroundColorFooter;
        border: 3px solid $colorChange;
        color: $colorTitle;
      }
    }
  }
}


</style>

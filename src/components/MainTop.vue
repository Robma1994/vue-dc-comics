<template>
  <div class="container-large">
    <div class="container-small">
      <MainFumetti 
        v-for="(cartoon,index) in comicBooks" 
        :key="index"
        :cart= cartoon
      />
      
    </div>
  </div>
</template>

<script>
import dcComics from '@/assets/data/dcComics.js'
import MainFumetti from '@/components/MainFumetti.vue'
export default {
  name: 'MainTop',
  components: {
    MainFumetti
  },
  data() {
    return {
      comicBooks: dcComics
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/Variables";
.container-large {
  background-color: white;
}
.container-small {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

</style>

<template>
  <div class="container-large">
    <div class="container-small header-horizzontal ">
      <div>
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index" >
            <a :class="(link.current == true) ? 'active' : null"  href="#">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          text : "CHARACTERS",
          url : "#",
          current : false
        },
        {
          text : "COMICS",
          url : "#",
          current : true
        },
        {
          text : "MOVIES",
          url : "#",
          current : false
        },
        {
          text : "TV",
          url : "#",
          current : false
        },
        {
          text : "GAMES",
          url : "#",
          current : false
        },
        {
          text : "COLLECTIBLES",
          url : "#",
          current : false
        },
        {
          text : "VIDEOS",
          url : "#",
          current : false
        },
        {
          text : "FANSE",
          url : "#",
          current : false
        },
        {
          text : "NEWS",
          url : "#",
          current : false
        },
        {
          text : "SHOP",
          url : "#",
          current : false
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/Variables";

.header-horizzontal {
  display: flex;
  align-items: center;
}

.container-small {
  padding: 20px 0 20px 0;
  div {
      width: 20%;
  }
  nav {
      width: 80%;
    }
}

ul {
display: flex;
justify-content: flex-end;
list-style-type: none;

  li a {
    text-decoration: none;
    padding: 15px;
    font-size: 14px;
    color: $colorLink;
    font-weight: $fontWeight500;
  
    &:hover {
      color: $colorChange;
    }
    &.active{
      color: $colorChange;
      border-bottom: 5px solid $colorChange;
      padding-bottom: 60px;
    }
  }
}



</style>

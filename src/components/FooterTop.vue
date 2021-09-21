<template>
  <div class="container-large">
    <div class="container-small">
      <div class="footer-top-left">
        <div>
          <h1>DC COMICS</h1>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <div>
          <h1>SHOP</h1>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
        </div>
        </div>
        <div>
          <h1>DC</h1>
          <ul>
            <li>Terms of use</li>
            <li>Privacy policy(New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact US</li>
          </ul>
        </div>
        <div>
          <h1>SITE</h1>
          <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
        
      </div>
      <div class="footer-top-right">
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'FooterTop',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../components/style/Variables";
.container-large {
  background-image: url('../assets/img/footer-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
.container-small {

  &::after {
    clear: both;
    display: table;
    content: ""
  }
  .footer-top-left {
    float: left;
    width: 50%;
    display: flex;
    
    div{
      width: 40%;
      padding: 10px 0 10px 0;

      h1{
        color: $colorTitle;
        font-size: 25px;
        padding: 20px 0 20px 0;
      }
    }
      li {
        list-style-type: none;
        color: $colorList;
        font-size: 13px;
        padding-bottom: 4px;
      }
  }
  .footer-top-right{
    float: right;
    width: 50%;
  }
}

</style>

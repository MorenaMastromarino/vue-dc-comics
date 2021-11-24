<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="footer-links">

          <div class="column">
            <h3>dc comics</h3>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li> 
            </ul>

            <h3>shop</h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>      
            </ul>
          </div>

          <div class="column">
            <h3>dc</h3>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>

          <div class="column">
          <h3>sites</h3>
          <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
          </ul>
          </div>
          
        </div>

        <div class="footer-logo">
        <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
        </div>
      </div>
    </div>

    <div class="footer-bottom">
      <div class="container">

        <div class="button">sign-up now!</div>

        <div class="social-icons">
          <a href="#">follow us</a>
          <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook logo"></a>
          <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter logo"></a>
          <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube logo"></a>
          <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest logo"></a>
          <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope logo"></a>        
        </div>

      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/mixins.scss';
  @import '../assets/style/vars.scss';

  footer {
    .footer-top {
      @include center-flex(center);
      height: 370px;
      overflow: hidden;
      background-image: url(../assets/img/footer-bg.jpg);
      background-size: cover;
  
      .container{
        @include center-flex(between);
  
        .footer-links {
          display: flex;
  
          .column {
            width: 150px;
            h3 {
              margin-bottom: 20px;
              text-transform: uppercase;
              color: #fff;
            }
            ul {
              margin-bottom: 20px;
              a {
                line-height: 20px;
                font-size: 11px;
                color: $footer-text-color;
              }
            }
          }
        }

        .footer-logo {
          width: 45%;
        }
  
      }
    }
  
    .footer-bottom {
      height: 100px;
      background-color: #303030;
      .container {
        @include center-flex(between);
        height: 100%;
        .social-icons a {
          padding: 0 10px;
          text-transform: uppercase;
          font-weight: bold;
          color: $primary-color;
          img {
            width: 35px;
            vertical-align: middle;
          }
        }
      }
     
    }

  }
</style>
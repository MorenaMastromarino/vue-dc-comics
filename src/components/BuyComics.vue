<template>
  <section class="buy-comics">
    <ul>
      <li>
        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
        <a href="#">digital comics</a>
      </li>
      <li>
        <img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
        <a href="#">dc merchandise</a>
      </li>
      <li>
        <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
        <a href="#">subscription</a>
      </li>
      <li>
        <img src="../assets/img/buy-comics-shop-locator.png" alt="comic shop locator">
        <a href="#">comic shop locator</a>
      </li>
      <li>
        <img src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa">        
        <a href="#">dc power visa</a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: 'BuyComics',
  
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/mixins.scss';
  @import '../assets/style/vars.scss';

  .buy-comics{
    @include center-flex(center);
    height: 160px;
    background-color: $primary-color;
    color: #fff;
    li {
      display: inline-block;
      padding: 0 35px;
      img {
        width: 50px;      
        vertical-align: middle;
        margin-right: 10px;
      }
      a{
        text-transform: uppercase;
        color: #fff;
      }
    }
  }
</style>
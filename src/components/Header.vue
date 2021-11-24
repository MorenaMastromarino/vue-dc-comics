<template>
  <header class="container">

    <div class="logo">
      <a href="#">
      <img src="../assets/img/dc-logo.png" alt="dc logo">
      </a>
    </div>

    <nav>
      <ul>
        <li><a href="#">characters</a></li>
        <li><a class="active" href="#">comics</a></li>
        <li><a href="#">movies</a></li>
        <li><a href="#">tv</a></li>
        <li><a href="#">games</a></li>
        <li><a href="#">collectibles</a></li>
        <li><a href="#">videos</a></li>
        <li><a href="#">fans</a></li>
        <li><a href="#">news</a></li>
        <li><a href="#">shop</a></li>
      </ul>
    </nav>
   
  </header>
</template>

<script>
export default {
  name: 'Header',

}
</script>

<style lang="scss" scoped>
  @import '../assets/style/mixins.scss';
  @import '../assets/style/vars.scss';

  header {
    @include center-flex(between);
    height: 100px;

    img {
      width: 80px;
    }
    
    li {
      display: inline-block;               
      a {
        display: inline-block;
        line-height: 95px;        
        padding: 0 15px;        
        text-transform: uppercase;
        font-size: 12px;
        font-weight: bold;
        color: #464646;  
        &:hover,
        &.active {
          border-bottom: 5px solid $primary-color;
          color: $primary-color;
        }  
      }    
      
    }
  }
  
</style>
<template>
  <header class="container">

    <div class="logo">
      <a href="#">
      <img src="../assets/img/dc-logo.png" alt="dc logo">
      </a>
    </div>

    <nav>
      <ul>
        <li v-for="(link, index) in navLinks" :key="index">
          <a :class="{active: link.active}" :href="link.url">{{link.text}}</a>
        </li>        
      </ul>
    </nav>
   
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{
      navLinks:[
        {
          url: '/',
          text: 'characters',
          active: false,
        },
        {
          url: '/',
          text: 'comics',
          active: true,
        },
        {
          url: '/',
          text: 'movies',
          active: false,
        },
        {
          url: '/',
          text: 'tv',
          active: false,
        },
        {
          url: '/',
          text: 'games',
          active: false,
        },
        {
          url: '/',
          text: 'collectibles',
          active: false,
        },
        {
          url: '/',
          text: 'videos',
          active: false,
        },
        {
          url: '/',
          text: 'fans',
          active: false,
        },
        {
          url: '/',
          text: 'news',
          active: false,
        },
        {
          url: '/',
          text: 'shop',
          active: false,
        },
      ],
    }
  },

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
        color: lighten($secondary-color, 20%);  
        &:hover,
        &.active {
          border-bottom: 5px solid $primary-color;
          color: $primary-color;
        }  
      }    
      
    }
  }
  
</style>
<template>
  <div class="wrapper">
    <Header/>
    <Main/>
    <BuyComics/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import BuyComics from './components/BuyComics.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    BuyComics,
    Footer
  }
}
</script>

<style lang="scss">
@import './assets/style/general.scss';
@import './assets/style/utilities.scss';

.wrapper {
  min-width: 1300px;
}
</style>

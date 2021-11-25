<template>
  <main>
    <div class="jumbotron"></div>

    <div class="current-series">
      <div class="container">

        <SerieCard 
          v-for="(card, index) in cardsData"
          :key= "index"
          :cardImage= "card.thumb"
          :cardTitle= "card.series"
        />            

      </div>
    </div>

  </main>
</template>

<script>
import SerieCard from './SerieCard';
import cardsData from '../assets/data/cardsData'

export default {
  name: 'Main',

  components: {
    SerieCard
  },

  data(){
    return{
      cardsData,
    }
  }


}
</script>

<style lang="scss" scoped>
  @import '../assets/style/mixins.scss';
  @import '../assets/style/vars.scss';

  main {
    .jumbotron {
      height: 300px;
      background-image: url(../assets/img/jumbotron.jpg);
      background-size: cover;
    }    

    .current-series{
      background-color: darken($secondary-color, 8%);
      .container {
        @include flex-wrap();
        padding: 20px 0;         
      }
      
    }
  }
</style>
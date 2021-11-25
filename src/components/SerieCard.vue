<template>

  <div class="serie-card">

    <div class="image-box">
      <img :src="cardImage" :alt="cardTitle">
    </div>

    <h3>{{cardTitle}}</h3>   

  </div> 
  
</template>

<script>
export default {
  name: 'SerieCard',
  props: {
    cardImage: String,
    cardTitle: String,
  }
}
</script>

<style lang="scss" scoped>
   @import '../assets/style/vars.scss';

  .serie-card {    
    flex-basis: calc(100% / 6);
    border: 15px solid darken($secondary-color, 8%);
    color: #fff;
    .image-box {
      height: 200px;
      overflow: hidden;
      margin-bottom: 20px;
    }
    h3 {
      font-size: 14px;
      text-transform: uppercase;
    }
  }
</style>
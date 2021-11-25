<template>

  <div class="serie-card">
    <img :src="cardImage" :alt="cardTitle">
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
  .serie-card {    
    color: #fff;
    flex-basis: calc(100% / 6);
  }
</style>
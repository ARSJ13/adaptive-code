<template>
  <div class="item-title">
    <v-icon class='mt-1 mr-2 d-flex' :class=flex x-large>{{ icon }}</v-icon>
    <h2 :style=disable>{{ money }}</h2>
    <v-btn tile block depressed style="color: #fff" :color=color>{{ name }}</v-btn>
  </div>    
</template>

<script>
export default {
  name: 'Item',
  props: ['flex', 'icon', 'money', 'disable', 'name', 'color']
}
</script>

<style scoped>

  .item-title{
    width: 18%;
    margin: 0.2rem;
    background-color: #B0BEC5;
    box-sizing: border-box;
  }
  .item-title h2{
    color: #37475F;
    margin-left: 10%;
    font-size: 250%;
    font-weight: 400;
  }

  @media screen and (max-width:1000px){
    .item-title{
      width: 30%;
    }
    h2{
      font-size: 0.7rem;
    }
  }
  @media screen and (max-width:600px){
    .item-title{
      width: 50%;
    }
  }
  @media screen and (max-width:400px){
    .item-title{
      width: 95%;
    }
    h2{
      font-size: 0.4rem;
    }
  }
</style>
<template>
  <v-col :style=style cols=col>
    <span>{{value}}</span>
    <span><v-icon style="color: #B0BEC5;" large>mdi-{{icon}}</v-icon> </span>
  </v-col>
</template>

<script>
export default {
  name: 'CalcButton',
  props: ['col', 'value', 'style', 'icon']
}
</script>

<style scoped>
  .col{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  span{
    color: #B0BEC5;
    font-size: 1.5rem;
  }
</style>
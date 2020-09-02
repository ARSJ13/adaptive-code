<template>
  <v-container class="d-flex justify-end align-center">
    <p class="user">Operador: {{user.name}} - {{user.date}} - {{user.hour}}</p>
    <span class="material-icons">help_outline</span>
    <span :class=icon></span>
  </v-container>
</template>

<script>
export default {
  name: 'User',
  data(){
    return {
      user: {
        name: 'Paulo César',
        date: '02/04/2018',
        hour: '19:37'
      },
      icon: 'icon'
    }
  }
}
</script>

<style scoped>
  .user{
    margin: 0;
    text-transform: uppercase;
    font-weight: 400;
  }
  .material-icons{
    margin: 0 0.4rem;
    font-size: 28px;
  }
  .icon{
    width: 24px;
    height: 24px;
    background-color: #43A047;
    border-radius: 50%;
  }

  @media screen and (max-width:450px){
    .user{
      font-size: 0.8rem;
    }
    .icon{
      width: 34px;
    }
  }
</style>
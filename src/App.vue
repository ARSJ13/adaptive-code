<template>
  <v-app id="inspire">
    <v-navigation-drawer v-model="drawer" app>
      <Calc />
    </v-navigation-drawer>

    <v-app-bar app color="#37475F" dark >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer">
        <span>
          <v-icon large>mdi-calculator</v-icon>
        </span>
      </v-app-bar-nav-icon>
      <User />
    </v-app-bar>

    <v-main>
      <v-container class="fill-height" fluid>
        <Content />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>

  import User from './components/User'
  import Content from './components/Content'
  import Calc from './components/Calc'

  export default {
    components: {
      User,
      Content,
      Calc
    },
    data: () => ({
      drawer: false,
    }),
  }
</script>

<style scoped>
*{
  font-family: 'Poppins', sans-serif;
}
.material-icons{
  font-size: 28px;
}
.fill-height{
  background-color: #CFD8DC;
  align-items: flex-end;
}

</style>

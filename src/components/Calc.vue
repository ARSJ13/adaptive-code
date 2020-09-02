<template>
    <v-container style="height:100%; padding: 0;" class="d-flex flex-column justify-space-between" fluid>
      <v-app-bar style="left:0;" color="#78909C" app>
        <span>
          <v-icon x-large color="#fff">mdi-account</v-icon>
        </span>
        <div class="user-title">
          <p>{{user.name}}</p>
          <p>{{user.cpf}}</p>
        </div>
      </v-app-bar>
      <div class="description">
        <p>Snack 100g 100 000001 100.001,20 100.001,20</p>
      </div>
      <div class="total">
        <v-row class="mr-0 ml-0 pl-1 pr-1 pt-1 d-flex justify-space-between" cols=4>
          <span>volumes</span>
          <span>total</span>
        </v-row>
        <v-row class="size mr-0 ml-0 pl-1 pr-1 pt-1 d-flex justify-space-between" cols=4>
          <span>01</span>
          <span>25,00
            <v-icon style="color: #37475F;" large>mdi-cash-register</v-icon>
          </span>
        </v-row>
      </div>
      <div class="calculator">
        <v-row class="calc-row ma-0 pa-2">
          <span class="pr-1">
            <v-icon style="color: #fff;" large>mdi-pin-outline</v-icon>
          </span>
          <span>
            <v-icon style="color: #fff;" large>mdi-text-box-search</v-icon>
          </span>
          <v-spacer></v-spacer>
          <span>
            <v-icon style="color: #fff;" large>mdi-view-grid</v-icon>
          </span>
        </v-row>
        <v-row style="height: 3rem">
        </v-row>
        <v-row class="ma-0">
          <CalcButton value=1 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=2 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=3 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=QTD col=3 style='background:#78909C; border: 0.5px solid #37474F;'/>  
        </v-row>
        <v-row class="ma-0">
          <CalcButton value=4 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=5 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=6 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton icon=backspace-outline col=3 style='min-width:74.88px; background:#78909C; border: 0.5px solid #37474F;'/>  
        </v-row>
        <v-row class="ma-0">
           <CalcButton value=7 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=8 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton value=9 col=3 style='background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton icon=arrow-bottom-left col=3 style='align-items:flex-end; padding-bottom: 0px; min-width:74.88px; background:#78909C; border: 0.5px solid #37474F; border-bottom: none;'/>  
        </v-row>
        <v-row class="ma-0">
           <CalcButton value=. col="3" style='background:#78909C; border: 0.5px solid #37474F;'/>
           <CalcButton value=0 col="6" style='min-width:120.60px; background:#546E7A; border: 0.5px solid #37474F;'/>
          <CalcButton col="3" style='min-width:74.88px; background:#78909C; border: 0.5px solid #37474F; border-top: none;'/>
        </v-row>
      </div>
    </v-container>
</template>

<script>
import CalcButton from './CalcButton'
export default {
  name: 'Calc',
  components: {
    CalcButton
  },
  data(){
    return {
      user: {
        name: "cliente padrão",
        cpf: '999.999.999-99'
      }
    }
  }
}
</script>

<style scoped>
  .user-title>p{
    margin: 0 0.6rem;
    font-size: 0.8rem;
    text-transform: uppercase;
    font-weight: bold;
    color: #fff;
  }
  .description{
    height: 40%;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  .description>p{
    padding-left: 0.3rem;
    font-size: 0.7rem;
    font-weight: bold;
    color: #78909C;
  }
  .total{
    background-color: #B0BEC5;
    width: 100%;
    height: 10%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .total span{
    text-transform: uppercase;
    font-weight: bold;
    font-size: 0.9rem;
    color: #37475F;
  }
  .size>span{
    font-size: 1.5rem;
  }
  .size>span:nth-child(2){
    color: #E64A19;
  }
  .calc-row{
    background-color: #37475F;
  }
  .calculator{
    border: 1px solid #37475F;
  }
</style>
<template>
  <v-container  class="d-flex flex-md-wrap flex-wrap justify-center align-center" fluid>
    <Item flex='justify-end' money='5,00' icon="mdi-cash-multiple" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='10,00' icon="mdi-cash-multiple" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='20,00' icon="mdi-cash-multiple" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='50,00' icon="mdi-cash-multiple" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='100,00' icon="mdi-cash-multiple" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='0,05' icon="mdi-currency-usd-circle-outline" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='0,10' icon="mdi-currency-usd-circle-outline" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='0,25' icon="mdi-currency-usd-circle-outline" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='0,50' icon="mdi-currency-usd-circle-outline" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='1,00' icon="mdi-currency-usd-circle-outline" name='selecione' color="#37475F" />
    <Item flex='justify-end' money='25,00' icon="mdi-cash-multiple" name='selecione' color="#546E7A" disable="color:#546E7A;"/>
    <Item flex='justify-end' money='26,00' icon="mdi-cash-multiple" name='selecione' color="#546E7A" disable="color:#546E7A;"/>
    <Item flex='justify-end' money='30,00' icon="mdi-cash-multiple" name='selecione' color="#546E7A" disable="color:#546E7A;"/>
    <Item flex='justify-end' money='40,00' icon="mdi-cash-multiple" name='selecione' color="#546E7A" disable="color:#546E7A;"/>
    <Item flex='justify-end' money='50,00' icon="mdi-cash-multiple" name='selecione' color="#546E7A" disable="color:#546E7A;"/>
    <Item flex='mb-8 mt-8' icon="mdi-cash-multiple" name='dinheiro' color="#E64A19" />
    <Item flex='mb-8 mt-8' icon="mdi-credit-card-multiple-outline" name='cartão crédito' color="#E64A19" />
    <Item flex='mb-8 mt-8' icon="mdi-credit-card-outline" name='cartão débito' color="#E64A19" />
    <Item flex='mb-8 mt-8' icon="mdi-subtitles-outline" name='cheque' color="#E64A19" />
    <Item flex='mb-8 mt-8' icon="mdi-arrow-right" name='próxima página' color="#37475F" />
  </v-container>
</template>

<script>

import Item from './Item'

export default {
  name: 'Content',
  components: {
    Item
  }
}
</script>

<style>
  
</style>
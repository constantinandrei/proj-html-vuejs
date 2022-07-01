<template>
  <div id="app">
    <TheNav></TheNav>
    <TheHeader></TheHeader>
    <TheMain></TheMain>
    <TheFooter></TheFooter>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheMain from './components/TheMain.vue';
import TheFooter from './components/TheFooter.vue';
import TheNav from './components/TheNav.vue';


export default {
  name: 'App',
  components: {
    TheHeader,
    TheMain,
    TheFooter,
    TheNav
},
  created(){
    document.title = 'Mareé | Constantin Andrei Todirascu'
  }
}
</script>

<style lang="scss">
  @import './assets/scss/variables.scss';
  @import './assets/scss/main.scss'
</style>

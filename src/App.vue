<template>
  <div id="app">
    <myHeader/>
    <myMain/>
    <myFooter/>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import myMain from './components/myMain.vue'
import myFooter from './components/myFooter.vue'


export default {
  name: 'App',
  components: {
    myHeader,
    myMain,
    myFooter,
  },

  data(){
    return{

    }
  }
}
</script>

<style lang="scss">
#app{
  font-family: 'Open Sans';
}
</style>

<template>
  <div id="app">
    <router-view></router-view>
    <FooterGuide v-show="$route.meta.showFooter"/>
  </div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide.vue'
import {mapActions} from 'vuex'
//import {reqFoodTypes} from './api'
export default {
  name: 'App',
  components: {
    FooterGuide
  },
  mounted(){
   //this.$store.dispatch('getAddress')
   this.getAddress(),
   this.getUserInfo()
  },
  methods:{
    ...mapActions(['getAddress','getUserInfo'])
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .app
    width 100%
    height 100%
    background #f5f5f5
</style>

<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script>
import Main from './components/Main.vue'
import vueSmoothScroll from 'vue2-smooth-scroll'
import StarRating from 'vue-star-rating'
import Vue from 'vue'
import BV from 'bootstrap-vue'

Vue.use(vueSmoothScroll)
Vue.use(StarRating)
Vue.use(BV)
Vue.component('star-rating', StarRating)

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style>
</style>

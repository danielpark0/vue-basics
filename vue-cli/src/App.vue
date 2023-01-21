<template>
  <div>
    <app-header 
    v-bind:propsdata="str"
    v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

// var AppHeader = {
//   template: '<header><h1></h1></header>'
// }

export default {
  data: function() {
    return {
      str: 'Header'
    }
  },
  components: {
    'app-header': AppHeader
  },
  methods: {
    renewStr: function() {
      this.str = 'hi';
    }
  }
}
</script>

<style>

</style>
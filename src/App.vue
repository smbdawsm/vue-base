<template>
  
  <div id="app">
      <component :is="layout">
        <router-view/>
      </component>
  </div>
</template>

<script>
import EmptyLayout from '@/layouts/EmptyLayout'
import MainLayout from '@/layouts/MainLayout'
//import './assets/jquery.min.js'
export default {
  computed: {
    layout() {
      console.log(this.$route.meta.layout)
      return this.$route.meta.layout + '-layout'
    }
  },
  components: {
    EmptyLayout, MainLayout
  }
}
</script>
<style lang="scss">
@import '~bootstrap/dist/css/bootstrap.css';
@import 'assets/bootstrap.min.css';
@import 'assets/index.css';
</style>
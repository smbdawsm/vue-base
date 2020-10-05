<template>
  
  <div id="app">
      <component :is="layout">
        <router-view />
      </component>
  </div>
</template>

<script>
import EmptyLayout from '@/layouts/EmptyLayout'
import MainLayout from '@/layouts/MainLayout'
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
@import 'assets/Login-Form-Dark.css';
@import 'assets/Header-Dark.css';
@import 'assets/index.css';
@import 'assets/css/Sidebar-Menu-1.css';
@import 'assets/Sidebar-Menu.css';
</style>
<template>
  <div id="app">
    
    <NavigationBar />

   
    <preNavigationBar />
  </div>
</template>

<script>
import NavigationBar from './components/navbar.vue'
import preNavigationBar from './components/prenavbar.vue'
  export default {
    name: 'App',
    components: {
      NavigationBar,
      preNavigationBar
    }
  }

</script>
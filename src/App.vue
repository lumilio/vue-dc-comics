<template>
  <div id="app">
    <C1/>
    <C2/>
    <C3/>
    <C4/>
    <C5/>
  </div>
  
</template>




<script>

import C1 from './components/Headermenu.vue'
import C2 from './components/Contentbox.vue' 
import C3 from './components/Banner.vue' 
import C4 from './components/Listbox.vue' 
import C5 from './components/Footermenu.vue'  

export default {
  name: 'App',
  components: {
      C1,
      C2,
      C3,
      C4,
      C5,
  }
}
</script>






<style lang="scss">

#app {
    @import './assets/scss/variables.scss';
    background-color: $sie-color-1;
}

</style>

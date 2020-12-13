<template>
  <div id="app">
    <NavigationBar />
    <router-view/>
  </div>
  
</template>

<script>
import NavigationBar from '@/components/NavigationBar.vue'
export default {
  name: "App",
  components: {
    NavigationBar
  }
}
</script>


<style>
  @import url('https://fonts.googleapis.com/css2?family=Hind+Siliguri&display=swap');

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'Hind Siliguri', sans-serif;
  }
  
</style>


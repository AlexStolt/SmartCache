<template>
  <div>
    <div id="navigation-bar">
      <img src="@/assets/logo.png" alt="" id="logo-image">
    </div>
    <h1 id="logo-header">Smart Cache</h1>
    
  </div>
</template>

<script>
export default {
  name: 'NavigationBar'
}
</script>


<style scoped>
  #navigation-bar {
    width: 100vw;
    height: 4vw;
    background-color: rgb(51, 51, 51);
  }

  #logo-image {
    position: fixed;
    top: 0.8vw;
    right: 0;
    left: 0;
    margin: 0 auto;
    width: 6vw;
    -webkit-box-shadow: 0.2vw 0.2vw 10px rgb(44, 44, 44);
    -moz-box-shadow:    0.2vw 0.2vw 10px rgb(44, 44, 44);
    box-shadow:         0.2vw 0.2vw 10px rgb(44, 44, 44);
    border: 1px solid rgb(158, 158, 158);
    background-color: rgb(255, 255, 255);
  }

  #logo-header {
    margin-top: 4vw;
    text-align: center;
    font-weight: 300;
    font-size: 2vw;
  }

</style>

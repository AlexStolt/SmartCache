<template>
  <div class="home">
    <div id="button-container">
      <router-link to="/global/files/" class="view-redirect-link">Global Files</router-link>
      <router-link to="/global/clipboard/" class="view-redirect-link">Global Clipboard</router-link>
      <router-link to="/private/files/" class="view-redirect-link" v-if="true">Private Files</router-link>
      <router-link to="/private/clipboard/" class="view-redirect-link" v-if="true">Private Clipboard</router-link>
    </div>
  </div>
</template>

<script>



export default {
  name: 'Home',
  components: {
    
  }
}
</script>
  

<style scoped>

  #button-container {
    display: grid;
    justify-content: center;
    grid-auto-rows: 4vw;
    grid-template-columns: repeat(2, 20vw);
    row-gap: 4vw;
    column-gap: 4vw;
    text-align: center;
    margin-top: 6vw;
  }

  .view-redirect-link {
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.2vw;
    color: black;
    text-decoration: none;
    background:rgb(255, 168, 168);
    box-shadow: 0.2vw 0.2vw 10px rgb(44, 44, 44);
    -webkit-transition: background 0.6s; /* For Safari 3.0 to 6.0 */
    transition: background 0.6s; /* For modern browsers */
  }

  .view-redirect-link:hover {
    background: #F66B6B;
  }

</style>

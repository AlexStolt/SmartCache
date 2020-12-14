<template>
  <div class="home">
    <div id="button-container">
      <router-link to="/global/files/" class="view-redirect-link">
        <img src="@/assets/folder.png" alt="" class="view-link-image">
        <p class="view-link-text">Global Files</p>
      </router-link>
      <router-link to="/global/clipboard/" class="view-redirect-link">
        <img src="@/assets/clipboard.png" alt="" class="view-link-image">
        <p class="view-link-text">Global Clipboard</p>
      </router-link>
      <router-link to="/private/files/" class="view-redirect-link" v-if="true">
        <img src="@/assets/folder-locked.png" alt="" class="view-link-image">
        <p class="view-link-text">Private Files</p>
      </router-link>
      <router-link to="/private/clipboard/" class="view-redirect-link" v-if="true">
        <img src="@/assets/clipboard-locked.png" alt="" class="view-link-image">
        <p class="view-link-text">Private Clipboard</p>
      </router-link>
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
    grid-template-columns: repeat(2, 14vw);
    row-gap: 4vw;
    column-gap: 4vw;
    margin-top: 6vw;
  }

  .view-redirect-link {
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    color: black;
    background: #f1f1f1;
    border: 1px solid rgb(73, 73, 73);
    box-shadow: 0.2vw 0.2vw 10px rgb(44, 44, 44);
    -webkit-transition: background 0.6s;
    transition: background 0.6s;
  }
  
  .view-redirect-link:hover {
    background: #cfcfcf;
  }


  .view-link-image {
    vertical-align: middle;
    width: 1.8vw;

  }

  .view-link-text {
    margin: 0.8vw;
    font-size: 1.2vw;
  }


</style>

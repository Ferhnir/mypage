<template>
 <div class="body-bg"></div>
</template>

<script>
export default {
  name: 'pageBackground'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 .body-bg {
   padding: 0px;
   margin: 0px;
   position: fixed;
   top: 0px;
   left: 0px;
   right: 0px;
   bottom: 0px;
   height: 100vh;
   width: 100vw;
   display: block;
   background: url('../assets/background-page.jpg') no-repeat fixed center center;
   background-size: cover;
   z-index: -100;
 }
</style>

<template>
  <div>
    <div class="container d-flex justify-content-center">
    <img height="200px" width="200px" class="eye" src="../assets/eye.png" alt="">
    <img height="200px" width="200px" class="cap" src="../assets/cap.png">
    </div>
    <!-- <div class="container d-flex justify-content-center eye">
    <img height="250px" width="250px" src="../assets/cap.png" alt="">
    </div> -->
  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.eye{
  margin-top: 250px;
  z-index: 1;
}
img {
  position: absolute;
  top: 25px;
  left: 25px;
}
.cap{
  z-index: 1;
}
</style>
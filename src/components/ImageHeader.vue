<template>
  <div class="image-header">
    <img src="../assets/ImageHeader.jpg" alt="image-header here">
    <div class="msg-text">{{ msg }}</div>
  </div>
</template>

<script>
export default {
  name: 'ImageHeader',
  props: {
    msg: String
  }
}
</script>

<style scoped>

img {
  width: 100%;
}
.msg-text {
  font-size: 2rem;
  font-weight: 600;
  font-family: cursive;
}
.image-header {
  
}
</style>
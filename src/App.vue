<template>
  <div id="app">
      <Header/>
    <router-view/>
  </div>
</template>
<script>
import Header from './components/layouts/Header.vue'

export default {
  name: "app",
  components: {
    Header
  }
}
</script>



<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
.btn {
  display: inline-block;
  border: none;
  background: #555;
  color: #fff;
  padding: 7px 20px;
  cursor: pointer;
}
.btn:hover {
  background: #666;
}
</style>


<!-- TODO add v-bind property to this element and 
bind dthis to text on the background picture so they are dynamic -->
<!-- TODO style the input box and add container class
make into a blog app for posting -->


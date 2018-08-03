<template>
  <div id="app" class="container">
    <app-preview-list></app-preview-list>
  </div>
</template>

<script>
import AppPreviewList from './components/AppPreviewList';

export default {
  name: "app",
  components: {
    AppPreviewList
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display:flex;
  flex-direction:column;
}
  .container{
    width:900px;
    margin:0 auto;
  }
</style>

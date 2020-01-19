<template>
  <div id="app">
    <Header logo="logo.png" />
    <MainContent />
  </div>
</template>

<script>
import Header from "./components/main/Header.vue";
import MainContent from "./components/MainContent.vue";


export default {
  name: "app",
  components: {
    Header,
    MainContent
  }
};
</script>

<style lang="sass">
body
  margin: 0
  padding: 0
#app
  font-family: 'Montserrat', sans-serif
  -webkit-font-smoothing: antialiased
  -moz-osx-font-smoothing: grayscale
</style>

<template>
  <div id="App">        
    <Header/>
    <SectionHeader/>    
    <Images/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import SectionHeader from './components/SectionHeader.vue'
import Images from './components/Images.vue'


  export default {
    name: 'App',
    components: {
      Header,
      SectionHeader,
      Images
    }
  }
</script>

<style>
#App {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

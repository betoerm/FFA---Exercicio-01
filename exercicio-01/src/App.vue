<template>
  <div id="app">        
    <Header/>
    <SectionHeader/>
    <Images/>
    <Article/>
    <SectionSide/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import SectionHeader from './components/SectionHeader.vue'
import Article from './components/Article.vue'
import SectionSide from './components/SectionSide.vue'
import Images from './components/Images.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionHeader,
    Images,
    Article,
    SectionSide
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

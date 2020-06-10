<template>
  <div id="app">
    <Header/>
    <Banner/>
    <Content :contentInfo="contentInfo"/>
    <Footer/>    
  </div>
</template>

<script>
import Header from './components/Header'
import Banner from './components/Banner'
import Content from './components/Content'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Banner,
    Content,
    Footer
  },
    data () {
      return {
        contentInfo: null
      }
  },
  mounted () {
    fetch('http://jsuol.com.br/p/pp/teste-front/data.json')
    .then(response => response.json() )
    .then(data => {
      this.contentInfo = data
    })
  }
}
</script>

<style>

</style>


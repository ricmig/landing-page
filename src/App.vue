<template>
  <div id="app" data-offset="100">
    <Header/>
    <Banner/>
    <Content/>
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
        info: null
      }
  },
  mounted () {
    fetch('http://jsuol.com.br/p/pp/teste-front/data.json')
    .then(response => response.json() )
    .then(data => {
      this.info = data
    })
  }
}
</script>

<style>

</style>


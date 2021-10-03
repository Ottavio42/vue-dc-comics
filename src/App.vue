<template>
  <div id="app">
    <Header/>
    <main>
      <Content/>
      <MarketingLinks/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Content from './components/Content.vue';
import MarketingLinks from './components/MarketingLinks.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Content,
    MarketingLinks,
    Footer
  }
}
</script>

<style lang="scss">
  @import "./assets/style/common";
</style>

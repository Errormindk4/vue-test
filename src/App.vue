<template>
  <div id="app">
    <Header />
    <SearchFullWidth />
    <SliderSection title="Elected Validators" :items="items" />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/common/Header";
import Footer from "@/components/common/Footer";
import SearchFullWidth from "@/components/pages/home-page/SearchFullWidth";
import SliderSection from "@/components/pages/home-page/SliderSection";

export default {
  name: 'App',
  data () {
    return {
      items: [
        {image: {}, title: 'test'},
        {image: {}, title: 'test'},
        {image: {}, title: 'test'},
        {image: {}, title: 'test'}
      ]
    }
  },
  components: {
    SliderSection,
    SearchFullWidth,
    Footer,
    Header
  }
}
</script>

<style lang="scss">
body, html {
  margin: 0;
  font-size: 14px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: linear-gradient(0, #fff, $main);
  padding: 0 40px;
}
</style>

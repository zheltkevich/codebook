<template>
  <div id="app">
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from '@/components/Header'
import Main from '@/components/Main'
import Footer from '@/components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
#app {
  display: flex;
  flex-direction: column;
  max-width: 100%;
  min-height: 100vh;
}

.container {
  max-width: 1220px;
  margin: 0 auto;
  padding: 0 10px;
  @media (min-width: 768px) {
    padding: 0 20px;
  }
  @media (min-width: 1280px) {
    padding: 0;
  }
}
</style>

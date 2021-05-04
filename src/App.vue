<template>
  <div id="app">
    <!-- HEADER -->
    <Header/>

    <!-- MAIN -->
    <main>main</main>

    <!-- FOOTER -->
    <footer>footer</footer>

  </div>
</template>

<script>
import Header from '@/components/Header.vue';

export default {
  name: 'App',
  components: {
    Header
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 10px;
}
#app {
  height:100vh;
}
.container{
  width: 1000px;
  height: 100%;
  margin: 0 auto;
}
</style>

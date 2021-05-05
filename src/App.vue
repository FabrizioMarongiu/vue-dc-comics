<template>
  <div id="app">
    <!-- HEADER -->
    <Header/>

    <!-- MAIN -->
    <Main />

    <!-- FOOTER -->
    <footer>footer</footer>

  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
   
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
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

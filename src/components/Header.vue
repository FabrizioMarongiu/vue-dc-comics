<template>
  <header class="header">
      <div class="container">
          <img class="logo" src="../assets/dc-comics-assets/img/dc-logo.png" alt="Dc Logo">



      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return {
             menu: [
                 {
                     dir: 'characters',
                     visible: false,
                 },
                 {
                     dir: 'comics',
                     visible: false,
                 },
                 {
                     dir: 'movies',
                     visible: false,
                 },
                 {
                     dir: 'tv',
                     visible: false,
                 },
                 {
                     dir: 'games',
                     visible: false,
                 },
                 {
                     dir: 'collectibles',
                     visible: false,
                 },
                 {
                     dir: 'video',
                     visible: false,
                 },
                 {
                     dir: 'fans',
                     visible: false,
                 },
                 {
                     dir: 'news',
                     visible: false,
                 },
                 {
                     dir: 'shop',
                     visible: false,
                 },
             ]
        }
    }
}
</script>

<style>
    .header{
        width: 100%;
        height:100px;
        background-color:aquamarine;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .logo{
        width:60px
    }




</style>
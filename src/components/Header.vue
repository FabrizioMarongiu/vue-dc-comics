<template>
  <header class="header">
      <div class="container flex-sb">
          <img class="logo" src="../assets/dc-comics-assets/img/dc-logo.png" alt="Dc Logo">

          <ul class="menu">
              <li class="choice"
            v-for="(element, index) in menu" :key="index">
            {{ element.dir }}</li>
              
          </ul>


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
    }
    .flex-sb{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .logo{
        width:60px
    }
    .menu{
        display: flex;
        height: 100%;
    }
    .choice{
        list-style: none;
        text-transform: uppercase;
        margin: 0 10px;
        color: #5f6673;
        display: flex;
        align-items: center;
        cursor: pointer;
        border-bottom: 2px solid transparent;
    }
    
    .choice:hover{
        color:#1684f9;
        border-bottom: 2px solid #1684f9;
    }

</style>
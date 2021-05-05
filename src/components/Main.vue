<template>
  <main class="main">
    <div class="jumbo">
        <img src="@/assets/dc-comics-assets/img/jumbotron.jpg" alt="">
    </div>

    <div class="jumbo-btm">
        <div class="container">
                    <a href="#" class="btn">current series</a>

            <div class="comics">
                <Cards 
                v-for="(element, index) in immagini"
                :key="index" 
                :immagine="element" />
                <!-- <div class="card">
                    <div class="img-box">
                         <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt=""> 
                    </div>
                    <span class="img-text">action comix</span>
                </div> -->
                
                
                
            </div>
        
        </div>

    </div>
   
    <div class="blue-section">
        <div class="flex-col container">
            <div class="card-icon"
            v-for="(element, index) in link"
            :key="index">
                <img class="w50" :src= " element.img " alt="Logo">
                <span class="card-text" >{{ element.nome }}</span>
             </div>
                    <!-- <div class="card">
                        <img class="w50" src="@/assets/dc-comics-assets/img/buy-comics-digital-comics.png" alt="">
                        <span class="card-text" >digital comics</span>
                    </div>
                    <div class="card">
                        <img class="w50" src="@/assets/dc-comics-assets/img/buy-comics-merchandise.png" alt="">
                        <span class="card-text" >digital comics</span>
                    </div>
                    <div class="card">
                        <img class="w50" src="@/assets/dc-comics-assets/img/buy-comics-subscriptions.png" alt="">
                        <span class="card-text" >digital comics</span>
                    </div>
                    <div class="card">
                        <img class=" w30" src="@/assets/dc-comics-assets/img/buy-comics-shop-locator.png" alt="">
                        <span class="card-text" >digital comics</span>
                    </div>
                    <div class="card">
                        <img class="w50" src="@/assets/dc-comics-assets/img/buy-dc-power-visa.svg" alt="">
                        <span class="card-text" >digital comics</span>
                    </div> -->
        </div>         
    </div>
      
  </main>
</template>

<script>
import Cards from '@/components/Cards.vue';
import imgComics from '@/data/imgComics.js';

export default {
    name:'Main',
    components: {
        Cards,
    },
    data(){
        return {
            link: [
                {
                    nome: 'digital comics',
                    img: require('@/assets/dc-comics-assets/img/buy-comics-digital-comics.png'),
                },
                {
                    nome: 'dc merciandise',
                    img: require('@/assets/dc-comics-assets/img/buy-comics-merchandise.png'),
                },
                {
                    nome: 'subscription',
                    img: require('@/assets/dc-comics-assets/img/buy-comics-subscriptions.png'),
                },
                {
                    nome: 'comic shop locator',
                    img: require('@/assets/dc-comics-assets/img/buy-comics-shop-locator.png'),
                },
                {
                    nome: 'dc power visa',
                    img: require('@/assets/dc-comics-assets/img/buy-dc-power-visa.svg'),
                },
            ],
            immagini: imgComics,


        }
    }
}
</script>

<style scoped lang="scss">
    .w30{
        width: 30px;
    }
    .w50{
        width: 50px;
    }
    .blue-section{
        width: 100%;
        height: 150px;
        background-color: #0282f9;
    }
    .flex-col{
        display: flex;
        justify-content: space-between;
    }
    .card-icon{
        display: flex;
        align-items: center;
        width: 100%;
        margin: 0 20px;
    }
    .card-text{
        color: white;
        text-transform: uppercase;
        margin-left: 20px;
    }

    .jumbo{
        overflow: hidden;
        height:300px;
        
    }
    .jumbo img{
        width: 100%;
        height: auto;
        object-fit: cover;
        position: relative;
        top: 0;
    }
    .jumbo-btm{
        height:500px;
        background-color: #1c1c1c;
        padding: 20px;
        position: relative;
    }
    .comics{
        width: 100%;
        display: flex;
        flex-wrap: wrap;
    }

    .btn{
        display:inline-block;
        width: 200px;
        height: 50px;
        background-color: #0282f9;
        text-transform: uppercase;
        position: absolute;
        text-decoration: none;
        text-align: center;
        font-size: 20px;
        padding: 13px;
        color: white;
        left: 200px;
        top: -25px;
        z-index: 10;
        &:hover{
            text-decoration: none;
            background-color: #4e91cf;
        }
    }
    
    /* .card {
        flex-basis: calc( 100% / 6 - 20px );
        margin: 0 10px;
        display: flex;
        flex-direction: column;
        
    }

    .img-box{
        overflow: hidden;
        width: 100%;
        height: 150px;
    }

    .img-box img{
        width: 100%;
    }

    .img-text{
        color: white;
        text-transform: uppercase;
    } */
  

    
</style>
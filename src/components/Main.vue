<template>
  <main class="main">
      <div class="text">
          <div class=" container">
        --> content goes here
          </div>
        </div>
          <div class="blue-section">
              <div class="flex-col container">
                  <div class="card"
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
export default {
    name:'Main',
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
            ]


        }
    }
}
</script>

<style>
    .text{
        width: 100%;
        height:100px; 
        background-color: #1c1c1c;
        color:white;
        font-size: 50px;
    }
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
    .card{
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
</style>
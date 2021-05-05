<template>
    <div class="card">
        <div class="img-box">
                <img :src="immagine.thumb"> 
        </div>
        <span class="img-text"> {{ immagine.series}} </span>
    </div>
</template>

<script>
export default {
    name: 'cards',
    props: ['immagine'],
}
</script>

<style>
    .card {
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
    }
</style>
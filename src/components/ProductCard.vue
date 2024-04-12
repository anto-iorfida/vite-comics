<script>
    export default {
        name: "ProductCard",
        props:{
            cardInfo: Object
        }
    } 
</script>

<template>
    <div class="card">
        <div class="contenitor-img">
            <img :src="cardInfo.thumb" >
        </div>
        <h4>{{cardInfo.series}}</h4>
    </div>

</template>

<style lang="scss" scoped>
    .card{
        width: calc(100% / 6 - 20px);
        margin: 10px;
        .contenitor-img{
            height: 80%;
            overflow: hidden;

            img{
                object-fit: cover;
                height: 100%;
            }
        }
        
        h4{
            text-transform: uppercase;
            color: lightgray;
            margin-top: 20px;
            font-size: small;
        }
    }

</style>
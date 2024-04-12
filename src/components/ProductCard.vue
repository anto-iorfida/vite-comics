<script>
    export default {
        name: "ProductCard",
        // props object in AppContentCentral
        props:{
            cardInfo: Object
        }
    } 
</script>

<!-- single card in AppContentCenter -->
<template>
    <div class="card">
        <div class="contenitor-img">
            <img :src="cardInfo.thumb" >
        </div>
        <h4>{{cardInfo.series}}</h4>
    </div>
</template>

<!--scss single card in AppContentCenter -->
<style lang="scss" scoped>
    .card{
        width: calc(100% / 6 - 20px);
        margin: 10px;
        &:hover {
                    transform: scale(1.1); 
                    transition: transform 0.3s ease-in-out; 
                    cursor: pointer;
                }
        .contenitor-img{
            height: 70%;
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
            font-weight: 400;
        }
    }

</style>
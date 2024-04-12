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
        <div>
            <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" >
        </div>
        <h4>miau</h4>
    </div>

</template>

<style lang="scss" scoped>
    .card{
        width: calc(100% / 6 - 20px);
        margin: 10px;
    }

</style>
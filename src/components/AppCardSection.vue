<script>
export default {
	name: 'AppCardSection',
    data(){
        return{
           cards:[
            {
                name:'DIGITAL COMICS',
                img: 'buy-comics-digital-comics.png'
            },
            {
                name:'DC MERCHANDISE',
                img: 'buy-comics-merchandise.png'
            },
            {
                name:'SUBSCRIPTION',
                img: 'buy-comics-subscriptions.png'
            },
            {
                name:'COMIC SHOP LOCALTOR',
                img: 'buy-comics-shop-locator.png'
            },
            {
                name:'DC POWER VISA',
                img: 'buy-dc-power-visa.svg'
            }
            ]
        }
    },
    methods: {
            getImageUrl(name) {
                return new URL(`../assets/img/${name}`, import.meta.url).href;
            }
        }
}
</script>

<template>
<section>
    <div class="container-small">
        <ul class="d-flex align-center justify-around gap-10">
            <li class="d-flex align-center gap-5" v-for="card in cards">
                <div><img :src="getImageUrl(card.img)"></div>
                <p>{{ card.name }}</p>
            </li>
        </ul>
    </div>
</section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as*;
    section{
        background-color: $blu-primary;
        padding: 20px;
        ul{
            
            li{
        
                p{
                    font-size: x-small;
                    color: white;
                }
                img{
                    width: 30px;
                }
            }
        }
    }

</style>
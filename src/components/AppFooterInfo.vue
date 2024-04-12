<script>
    export default {
	name: 'AppFooterInfo',
    data(){
        return{
            iconSocial:[
                {img:'footer-facebook.png'},
                {img:'footer-periscope.png'},
                {img:'footer-pinterest.png'},
                {img:'footer-twitter.png'},
                {img:'footer-youtube.png'}
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
        <div class="container d-flex justify-between">
            <div>
                <a href="">SIGN-UP NOW!</a>
            </div>
            <div class="d-flex align-center gap-10">
                <h4>FOLLOW US</h4>
                <ul class="d-flex gap-10">
                    <li v-for="icon in iconSocial"><img :src="getImageUrl(icon.img)"></li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as*;
    section{
        background-color: #303030;
        padding: 20px;
        .container{
            div:first-child{
                padding: 6px;
                border: 4px solid $blu-primary;
                font-size: small;
                color: white;
                &:hover {
                    transform: scale(1.3); 
                    transition: transform 0.3s ease-in-out; 
                    cursor: pointer;
                }
            }
            div:last-child{
                color: $blu-primary;
                li{
                    
                    img{
                        height: 30px;
                        border-radius: 50%;
                        
                        &:hover {
                            transform: scale(1.3); 
                            transition: transform 0.3s ease-in-out; 
                            border: 3px solid white;
                            cursor: pointer;
                        }
                    };
                }
            }
        }
    }
</style>

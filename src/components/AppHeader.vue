<script>
export default {
	name: 'AppHeader',
        data(){
            return{
                links:[
                    {
                        name: 'CHARACTERS',
                        active: false
                    },
                    {
                        name: 'COMICS',
                        active: false
                    },
                    {
                        name: 'MOVIES',
                        active: false
                    },
                    {
                        name: 'TV',
                        active: false
                    },
                    {
                        name: 'GAMES',
                        active: false
                    },
                    {
                        name: 'COLLECTIBLES',
                        active: false
                    },
                    {
                        name: 'VIDEOS',
                        active: false
                    },
                    {
                        name: 'FANS',
                        active: false
                    },
                    {
                        name: 'NEWS',
                        active: false
                    },
                    {
                        name: 'SHOP',
                        active: false
                    }
                ]

            }
        } 
}
</script>

<template>
    <header >
        <div class="container d-flex justify-between align-center">
        <div>
            <img src="../assets/img/dc-logo.png" alt="logo">
        </div>
        <nav>
            <ul class="d-flex ">
                <li class="d-flex align-center actives" v-for="link in links">{{ link.name }}</li>
            </ul>
        </nav>
    </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as*;
    .container{
        height: 120px;
        img{
            width: 80px;
        }
        ul{
            gap: 10px;
        
            li{
                height: 120px;
                
            }
        }
        .actives{
                    border-bottom: 4px solid $blu-primary;
                    color: $blu-primary;
                }
        
    }
</style>

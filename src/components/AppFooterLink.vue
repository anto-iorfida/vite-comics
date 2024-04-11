<script>
    export default {
	name: 'AppFooterLink',
    data(){
            return{
                dcComics :[
                    { name: 'Characters' },
                    { name: 'Comics' },
                    { name: 'Movies' },
                    { name: 'Tv' },
                    { name: 'Games' },
                    { name: 'Collectibles' },
                    { name: 'Videos' },
                    { name: 'Fans' },
                    { name: 'News' },
                    { name: 'Shop' },
                ],
                shop:[
                    { name: 'Shop Dc'},
                    { name: 'Shop Dc Collaboration'}
                ],
                dc:[
                    { name: 'Terms Of Use'},
                    { name: 'Privacy policy(new)'},
                    { name: 'Ad Choices'},
                    { name: 'Advertising'},
                    { name: 'Jobs'},
                    { name: 'Subscriptions'},
                    { name: 'Talent Workshops'},
                    { name: 'CPSC Certificates'},
                    { name: 'Ratings'},
                    { name: 'Shop Help'},
                    { name: 'Contact Us'}
                ],
                sites:[
                    { name: 'DC'},
                    { name: 'MAD Magazine'},
                    { name: 'DC Kids'},
                    { name: 'DC Universe'},
                    { name: 'Dc Power Visa'}
                ]


            }
        } 
    }
</script>

<template>
<section >
    <div class="container d-flex gap-20">
        <div>
            <div>
                <h4>DC COMICS</h4>
                <ul>
                    <li v-for="singleLink in dcComics">{{ singleLink.name }}</li>
                </ul>
            </div>
            <div>
                <h4>SHOP</h4>
                <ul>
                    <li v-for="singleLink in shop">{{ singleLink.name }}</li>
                </ul>
            </div>
        </div>
        <div>
            <h4>DC</h4>
            <ul>
                <li v-for="singleLink in dc">{{ singleLink.name }}</li>
            </ul>
        </div>
        <div>
            <h4>SITES</h4>
            <ul>
                <li v-for="singleLink in sites">{{ singleLink.name }}</li>
            </ul>
        </div>
    </div>
</section>
</template>

<style lang="scss" scoped>
    section{
        padding: 20px 0;
        background-image: url('../assets/img/footer-bg.jpg');
        h4{
            color: white;
            font-size:medium;
        }
        ul{
            margin: 16px 0;
            li{
                color: gray;
                font-size: small;
                margin: 6px 0;
            }
        }
    }
</style>
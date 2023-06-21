<script>
    export default {
        data() {
            return {
                
                    DcComics:[
                        {
                        section : 'dc comics',
                        nome: 'Characters',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc comics',
                        nome: 'Comics',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc comics',
                        nome: 'Movies',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc comics',
                        nome: 'TV',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc comics',
                        nome: 'Games',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc comics',
                        nome: 'Videos',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc comics',
                        nome: 'News',
                        link: '#',
                        active: false,
                        },
                    ],
                    shop:[
                        {
                        section : 'shop',
                        nome: 'Shop DC',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'shop',
                        nome: 'Shop DC Collectible',
                        link: '#',
                        active: false,
                        },
                        
                    ],

                    dc:[
                        {
                        section : 'dc',
                        nome: 'Terms Of Use',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Privacy policy (New)',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Ad Choices',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Advertising',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Jobs',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Subscriptions',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Talent Workshops',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'CPSC Certificates',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Ratings',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Shop Help',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'dc',
                        nome: 'Contact Us',
                        link: '#',
                        active: false,
                        },

                    ],
                    sites:[
                        {
                        section : 'sites',
                        nome: 'DC',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'sites',
                        nome: 'MAD Magazine',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'sites',
                        nome: 'DC kids',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'sites',
                        nome: 'DC Universe',
                        link: '#',
                        active: false,
                        },
                        {
                        section : 'sites',
                        nome: 'DC Power Visa',
                        link: '#',
                        active: false,
                        },
                    ]
            }
        }
        
        
    }
</script>
<template >
    <div class="footer-container">
        <div class="macro-section container">
            <div class="row">
                <div class=" col-4">
                    <h3 class="text-center">DC COMICS</h3>
                    <div class="text-start" v-for="(comic, index) in DcComics" :key="index">
                        <ul>
                            <li><a href="">{{ comic.nome }}</a></li>
                        </ul>
                    </div>
                    <h3 class="text-center pe-4">SHOP</h3>
                    <div class="text-start" v-for="(shop, index) in shop" :key="index">
                        <ul>
                            <li><a href="">{{ shop.nome }}</a></li>
                        </ul>
                    </div>
                </div>
                <div  class="col-4">
                    <h3 class="text-center pe-5">DC</h3>
                    <div class="text-start" v-for="(dc, index) in dc" :key="index">
                        <ul>
                            <li><a href="">{{ dc.nome }}</a></li>
                        </ul>
                    </div>
                </div>
                <div  class="col-4">
                    <h3 class="text-center pe-5">SITES</h3>
                    <div class="text-start" v-for="(site, index) in sites" :key="index">
                        <ul>
                            <li><a href="">{{ site.nome }}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-bottom-bar">
            <div class="footer-content">
                <button>SIGN UP NOW!</button>
                <div class="footer-right-content">
                    <span class="d-none d-lg-inline">FOLLOW US</span>
                    <img src="/src/assets/footer-facebook.png" alt="">
                    <img src="/src/assets/footer-periscope.png" alt="">
                    <img src="/src/assets/footer-pinterest.png" alt="">
                    <img src="/src/assets/footer-twitter.png" alt="">
                    <img src="/src/assets/footer-youtube.png" alt="">
                </div>
            </div>
        </div>
        
    </div>
</template>
<style lang="scss" >
    .footer-container{
        background-image: url('/footer-bg.jpg');
        flex-direction: column;
        background-repeat: no-repeat;
        background-size: cover;
        
        
        .macro-section{
            display: flex;
            background-image: url('/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: right top 65%;   
                
        
                h3{
                    color: white;
                    padding-top: 1.5rem;
                }
                
                ul{
                    
                    a{
                        color: #959595;
                        font-size: 16px
                    };
                    }
                }
        

    }

    .footer-bottom-bar{
        width: 100%;
        height: 100px;
        background-color: #202020;
        
        
        .footer-content{
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
            padding: 0 10rem;

            button{
                background-color: transparent;
                border: 2px solid #0282F9;
                padding: 10px 15px;
                color:white;
            }

            .footer-right-content{
                display: flex;
                align-items: center;
                
                    span{
                        color: #0282F9;
                        margin: 0rem 0.5rem;
                    }

                    img{
                        margin: 0rem 0.275rem;
                    }
            }

        }
    }
    
</style>
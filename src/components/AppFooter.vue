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
        <div class="macro-section">
            <div class="section">
                <h3>DC COMICS</h3>
                <div v-for="(comic, index) in DcComics" :key="index">
                    <ul>
                        <li><a href="">{{ comic.nome }}</a></li>
                    </ul>
                </div>
                <h3>SHOP</h3>
                <div v-for="(shop, index) in shop" :key="index">
                    <ul>
                        <li><a href="">{{ shop.nome }}</a></li>
                    </ul>
                </div>
            </div>
            <div  class="section">
                <h3>DC</h3>
                <div v-for="(dc, index) in dc" :key="index">
                    <ul>
                        <li><a href="">{{ dc.nome }}</a></li>
                    </ul>
                </div>
            </div>
            <div  class="section">
                <h3>SITES</h3>
                <div v-for="(site, index) in sites" :key="index">
                    <ul>
                        <li><a href="">{{ site.nome }}</a></li>
                    </ul>
                </div>
            </div>
            
        </div>
        <div class="footer-bottom-bar">
            <div class="footer-content">
                <button>SIGN UP NOW!</button>
                <div class="footer-right-content">
                    <span>FOLLOW US</span>
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
            padding: 2rem 10rem;  
            background-image: url('/dc-logo-bg.png');
            width: 90%;
            background-repeat: no-repeat;
            background-position: right top 65%;   
                .section{
                    width: calc(60% / 3);
                }
        
                h3{
                    color: white;
                    padding-top: 1.5rem;
                }
                
                ul{
                    li{
                    padding: 0.3rem 0;
                    
                    a{
                        color: #959595;
                    };
                    }
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
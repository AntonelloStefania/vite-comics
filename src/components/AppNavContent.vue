<script>
    export default {
        data() {
            return {
                navLinks:[
                    {
                        section_name : 'digital comics',
                        section_icon : './src/assets/buy-comics-digital-comics.png',
                        active: false,
                        link:'#'
                    },
                    {
                        section_name : 'dc merchandise',
                        section_icon : './src/assets/buy-comics-merchandise.png',
                        active: false,
                        link:'#'
                    },
                    {
                        section_name : 'subscription',
                        section_icon : './src/assets/buy-comics-subscriptions.png',
                        active: false,
                        link:'#'
                    },
                    {
                        section_name : 'comic shop logator',
                        section_icon : './src/assets/buy-comics-shop-locator.png',
                        active: false,
                        link:'#'
                    },
                    {
                        section_name : 'dc power visa',
                        section_icon : './src/assets/buy-dc-power-visa.svg',
                        active: false,
                        link:'#'
                    },
                ]
            }
        },
        
    }
</script>


<template lang="">
    <div class="nav-container container">
        <ul>
            <li v-for="(navLink, index) in navLinks">
                <a :href="navLink.link">
                    <img :src="navLink.section_icon" alt="">
                    <span> {{navLink.section_name.toUpperCase()}}</span>
                </a>
            </li>
        </ul>
    </div>
</template>


<style lang="scss">

.nav-container{
    background-color:#0282F9;
    height: 150px;
    ul{ 
        display: flex;
        width: 100%;
        
        li{
            width: calc(100% / 5 );
            display: flex;
            align-items: center;
            
            a{
                display: flex;
                align-items: center;
               
                    img{
                    width: 50px;
                    height: 50px;
                    margin-right:0.5rem
                    }

                    span{
                        color: white;
                        font-weight: bold;
                    }

                
            }

        }
       

        
    }

}
    
</style>
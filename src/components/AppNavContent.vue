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
                        section_name : 'comic shop locator',
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
    <div class="nav-container">
        <div class="container">
            <div class="rowalign-items-center justify-content-between">
                <ul class="py-4  d-flex flex-column flex-md-row ">
                    <li class="d-flex col-12 col-md-auto py-3 py-lg-0" v-for="(navLink, index) in navLinks">
                        <a :href="navLink.link">
                            <img :src="navLink.section_icon" alt="">
                            <span class="d-inline d-md-none d-lg-inline"> {{navLink.section_name.toUpperCase()}}</span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>

.nav-container{
    background-color:#0282F9;
    ul{ 
        display: flex;
        justify-content: space-around;
        height: 100%;
        align-items: center;
        margin-bottom: 0rem;
        padding-left:0;
        
        
        li{
            height: 100%;
            
            
            a{
                display: flex;
                align-items: center;
                height: 100%;
               
                    img{
                    width: 50px;
                    height: 60px;
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
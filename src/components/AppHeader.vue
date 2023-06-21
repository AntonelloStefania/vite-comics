<script>
   export default{
    data(){
        return {
            links:[
                {
                   label : 'characters',
                   link : '#',
                   active : false,
                },
                {
                   label : 'comics',
                   link : '#',
                   active : false,
                },
                {
                   label : 'movies',
                   link : '#',
                   active : false,
                },
                {
                   label : 'tv',
                   link : '#',
                   active : false,
                },
                {
                   label : 'games',
                   link : '#',
                   active : false,
                },
                {
                   label : 'collectibles',
                   link : '#',
                   active : false,
                },
                {
                   label : 'videos',
                   link : '#',
                   active : false,
                },
                {
                   label : 'fans',
                   link : '#',
                   active : false,
                },
                {
                   label : 'news',
                   link : '#',
                   active : false,
                },
                {
                   label : 'shop',
                   link : '#',
                   active : false,
                },
            ],
            activeItem : -1,
        }
    }, methods: {
        getActiveItem(index){
            if (this.activeItem !== -1) {
                this.links[this.activeItem].active = false;
            }
            this.links[index].active = true;
            this.activeItem = index;
        },
    }
   }
</script>

<template >
    <div class="container header-container">
        <div class="row flex-column flex-lg-row align-items-center py-2">
            <div class="col-12 col-md-3 d-flex justify-content-center justify-content-lg-start">
                <img src="/dc-logo.png" alt="logo"/>
            </div>
            <div class="col d-none d-lg-block">
                <ul>
                    <li v-for="(link,index) in links" :key="index" @mouseover="getActiveItem(index)"> 
                        <a :class="links[index].active ? 'active': ''" :href="link.link">{{link.label.toUpperCase()}}</a> 
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style  lang="scss"  scoped>
.active{
    color: #0282F9;
    border-bottom: 6px solid #0282F9;
    padding-bottom: 40px;
}

.header-container{
    align-items: center;
    justify-content: space-between;
   
    img{
        width: 80px;
    }
        ul{
            li{
                display: inline;
                padding: 1rem;
                font-size: 15px;
                font-weight: bold;

            }
        }
}


 
</style>
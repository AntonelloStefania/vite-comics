<script>
    export default {
       props:{
         myCard : Object
        }
    }
</script>
<template>
    <div class="container ">
        <div >
            <a href=""><img :src="myCard.thumb" alt="" class="py-3"></a>
            <h6 class="pt-2 text-center pb-3">{{ myCard.series.toUpperCase() }}</h6>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    img{
        height: 300px;
        width:300px;
    }

    img:hover{
        opacity: 0.5;
    }

    h6{
        color:rgb(255, 255, 255);
        font-size: 12px;
    }
</style>
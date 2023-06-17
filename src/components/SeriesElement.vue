<template>
    <div class="series-container">
        <div class="image-container">
            <img :src="thumb" alt="">
        </div>
        <div class="title-container">
            <p>{{ series }}</p>
        </div>
        
    </div>
</template>
<script>
export default {
    name:"SeriesElement",
    props : {
        thumb : String,
        price : String,
        series : String,
        type : String
    }
}
</script>
<style>
.series-container{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        
    }
    .image-container{
        height: 170px;
        width: 170px;
    }
    .title-container{
        height: 80px;

    }
img{
    width:100%;
    height: 100%;
    object-fit: cover;
    
}
p{
    color:white;
    max-width: 150px;
}    
</style>
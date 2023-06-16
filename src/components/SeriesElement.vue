<template>
    <div class="series-container">
        <img :src="thumb" alt="">
        <p>{{ series }}</p>
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
        
    }
img{
    width:100px;
    height: 100px;
    object-fit: cover;
    
}
p{
    color:white;
}    
</style>
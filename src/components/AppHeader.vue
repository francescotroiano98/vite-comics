<template>
    <section class="container">

        <div class="logo-container">
            <img src="../assets/img/dc-logo.png" alt="">
            
        </div>
        <div>
            <nav>
                <ul>
                    <li v-for="list in dcNavList">{{ list }}

                    </li>
                </ul>
            </nav>
        </div>
    </section>    
</template>
<script>
export default {
    data(){

        return{

            dcNavList:[
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ]
            
        }
    }
    
}
</script>
<style lang="scss">
.container{
    padding-top: 0.5rem;
}
.logo-container img{
    width: 75%;
}
ul{
    display: flex;

}
li{
    margin-right: 1.6rem;
    font-size: 0.75rem;
}

</style>
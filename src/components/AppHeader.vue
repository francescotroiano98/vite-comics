<template>
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

</style>
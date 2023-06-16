<template>
    <main>
        <section class="main-top">

        </section>
        <section class="main-bottom">

           
                

                <Series/>

            

        </section>
        

        
    </main>       
    
</template>
<script>
import Series from './Series.vue';
export default {
        name:"AppMain",
        components : {
            Series
        }
}
</script>
<style lang="scss">
main{
    position: relative;
    z-index: 1;
    background-color: black;
    
    padding-bottom: 1rem;
 
}
h1{
    color: white;
}
.main-top{
    background-image: url(../assets/img/jumbotron.jpg);
    height: 350px;
    width: 100%;
    background-size: cover;
    
}
</style>
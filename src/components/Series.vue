<template>
    
        <section class="container">
            <div class="current-series">

                <h1>CURRENT SERIES
                    
                </h1>
            </div>
            
                <SeriesElement v-for="singleElement in seriesList" :thumb="singleElement.thumb" :series="singleElement.series"/>
                
                    <button>
                        LOAD MORE
                    </button>
                
       </section>
      
</template>
<script>
import SeriesElement from './SeriesElement.vue';
export default {
    name:"Series",
    components : {
        SeriesElement
    },
    data(){
        return{

            seriesList:[
                            {
                                "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                                "price": "$19.99",
                                "series": "Action Comics",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                                "price": "$3.99",
                                "series": "American Vampire 1976",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                                "price": "$16.99",
                                "series": "Aquaman",
                                "type": "graphic novel",
                            },
                            {
                                "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                                "price": "$2.99",
                                "series": "Batgirl",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                                "price": "$3.99",
                                "series": "Batman",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                                "price": "$2.99",
                                "series": "Batman Beyond",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                                "price": "$3.99",
                                "series": "Batman/Superman",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                                "price": "$4.99",
                                "series": "Batman/Superman Annual",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                                "price": "$5.99",
                                "series": "Batman: The Joker War Zone",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                                "price": "$6.99",
                                "series": "Batman: Three Jokers",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                                "price": "$4.99",
                                "series": "Batman: White Knight Presents: Harley Quinn",
                                "type": "comic book",
                            },
                            {
                                "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                                "price": "$16.99",
                                "series": "Catwoman",
                                "type": "graphic novel",
                            },
                        ]
        }

    }
}
</script>
<style scoped>
.current-series{
    position: absolute;
    bottom: 515px;
    left: px;
    background-color: blue;
    padding-left: 1.5rem;
    padding-right: 1.5rem;
}
.current-series h1{
    color: white;
    font-size: 0.9rem;
}
    .container{
        position: relative;
        flex-wrap: wrap;
        justify-content: space-between;
        padding-top: 3rem;
        padding-bottom: 2rem;
    }
    button{
        position: absolute;
        top: 100%;
        left: 50%;
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
        background-color: blue;
        color: white;
        padding: 0.7rem 3.5rem 0.7rem 3.5rem;
        
        border: 1px solid blue;
        
    }
</style>
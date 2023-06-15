<template>
    <footer>
        <section class="footer-top">
            <div class="container">

                <div class="left-nav-content">
                    <nav>
                        <ul>
                            <li v-for="(link) in footerLink">

                                    <h2>{{ link.name }}</h2>

                                <p v-for="(link) in link.link">

                                    {{ link }}
                                
                                </p>

                            </li>                           
                            
                        </ul>
                    </nav>
                </div>

                <div class="right-content">
                    <img src="../assets/img/dc-logo-bg.png" alt="">

                </div>


            </div>
            
        </section>
        <section class="footer-bottom">
            <section class="container">
                <div>
                    <button>SIGN-UP NOW!</button>
                </div>
                <div>
                    <nav>
                        <ul>
                            
                        </ul>
                    </nav>
                </div>
            </section>    
        </section>
    </footer>
</template>
<script>
export default {
    data(){
        
        return{

            
            footerLink:[{
                name: 'DC COMICS',
                link:[
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS'
                ]
                
            },
            {
                name: 'DC',
                link:[
                "CHARACTERS",
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS'
                ]
            },
            {
                name: 'SITES',
                link:[
                'CHARACTERS',
                'COMICS',
                'FANS',
                'NEWS'
                ]
            },
            {
                name: 'SHOP',
                link:[
                
                'COMICS',
                'MOVIES',
                'GAMES',
                'COLLECTIBLES',
                
                ]
            },
                
            ],
           
            
        }
    }
    
}
</script>
<style lang="scss" scoped>
.footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    
}
.footer-bottom{
    background-color: rgb(60, 60, 60);
    position: relative;
    z-index: 1;
    padding-top: 1rem;
    padding-bottom: 1rem;
    
}
button{
    padding: 0.5rem;
}
.left-nav-content{
    width: 50%;
}
.right-content{
display: flex;
align-items: center;
justify-content: center;
width: 50%;
}
.right-content img{

position: absolute;
width: 35%;

}
ul{
    display: flex;
    flex-wrap: wrap;
    padding: 0;
    min-width: 456px;
}
li{
    color: white;
    
    margin-right: 4rem;
}
li h2{
    margin-top: 0px;
    margin-bottom: 0.7rem;
}
li p{
    font-size: 0.5rem;
    color: white;   
}
    
</style>
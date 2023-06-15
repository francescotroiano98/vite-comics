<template>
    <footer>
        <section class="footer-top">
            <div class="container">

                <div class="left-nav-content">
                    <nav>
                        <ul>
                            <li v-for="link in footerLink">{{ link.name }} {{ link.link }}</li>
                        </ul>
                    </nav>
                </div>

                <div class="right-content">
                    <img src="../assets/img/dc-logo-bg.png" alt="">

                </div>


            </div>
            
        </section>
        <section class="footer-bottom">

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
                
            ]
        }
    }
    
}
</script>
<style lang="scss">
.footer-top{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    
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

width: 50%;

}
li{
    color: white;
}
    
</style>
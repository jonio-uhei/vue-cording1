<template>
    <header>
        <div class="container">
            <div class="header-flexbox">
                <h1>My Work</h1>
                <nav class="flex-box">
                    <ul
                        v-for="list in lists"
                        :key="list.id"
                    >
                        <a href="#"><li>{{list.title}}</li></a>
                        <a href="#"><img  class="flex-box__image" :src="list.image" alt=""></a>
                    </ul>
                </nav><!--/.flex-box-->
            </div><!--/.header-flexbox-->
        </div><!--/.container-->
        <img class="hero-smart" src="../assets/images/hero-smart.jpg" alt="">
        <img class="hero-pc" src="../assets/images/hero-pc.jpg" alt="">
        
    </header>
</template>

<script>
    export default{
        data:function(){
            return {
                lists:[
                    {
                        title:'About'
                    },
                    {
                        title:'Works'
                    },
                    {
                        title:'News'
                    },
                    {
                        title:'Contact'
                    },
                    {
                        image:require('@/assets/images/instagram.png'),
                    },
                ],
                
            };
        }
    }
</script>
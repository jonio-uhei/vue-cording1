<template>
    <main>
        <div>
            <div class="container">
                <section id="about">
                    <div class="section">
                        <h2 class="section__title">About</h2>
                        <p class="section__name">Xxxxx Ashley</p>
                        <ul>
                            <li
                                class="section__list"
                                v-for="list in lists"
                                :key="list.id"
                            >{{list.content}}</li>
                        </ul>
                        <p class="content">プロフィールテキストテキストテキストテキストテキストテキストテキストテキストテキストスト テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト</p><!--/.content-->
                    </div><!--/.about-->
                </section><!--/#about--> 
                <section id="works">
                    <div class="section">
                        <h2 class="section__title">Works</h2><!--/.sectoin__title-->
                        <div class="section__flexbox">
                            <img 
                                class="section__image"
                                v-for="image in images"
                                :key="image.id"
                                :src="image.image"
                            ><!--/.section__image-->
                        </div><!--/.section__flexbox-->
                    </div><!--/.about-->
                </section><!--/#works--> 
                <section id="news">
                    <div class="section">
                        <h2 class="section__title">News</h2>
                        <div class="section-wrap">
                            <ul
                                class="information"
                                v-for="information in informations"
                                :key="information.id"
                            ><!--/.information-->
                                <li>{{information.date}}</li>
                                <li>{{information.content}}</li>
                            </ul>
                        </div><!--/.section-wrap-->
                    </div><!--/.about-->
                </section><!--/#news--> 
                <section id="contact">
                    <div class="section">
                        <h2 class="section__title">Contact</h2>
                        <form class="contact" action="#" method="post">
                            <div class="contact__flexbox">
                                <p class="contact__title">NAME</p><!--/.contact__title-->
                                <input type="text" name="name">
                            </div><!--/.contact__flexbox-->
                            <div class="contact__flexbox">
                                <p class="contact__title">E-mail</p><!--/.contact__title-->
                                <input type="email" name="email">
                            </div><!--/.contact__flexbox-->
                            <div class="contact__flexbox">
                                <p class="contact__title">MESSAGE</p><!--/.contact__title-->
                                <textarea name="comment"></textarea>
                            </div><!--/.contact__flexbox-->
                            <input class="contact__submit" type="submit" value="送信">
                        </form><!--/.contact-->
                    </div><!--/.about-->
                </section><!--/#contact--> 
            </div><!--/.container-->
        </div>
    </main>
</template>

<script>
    export default{
        data:function(){
            return{
                lists:[
                    {
                        content:'2th Floor xxxxx Building x-x-x Nishiazabu, Minato-ku, Tokyo 106-0031 Japan'
                    },
                    {
                        content:'tel: 000-0000-0000'
                    },
                    {
                        content:'url: www.xxxxxx.jp'
                    },
                    {
                        content:'mail: xxx@xxxxxx.jp'
                    },
                ],
                images:[
                    {
                        image:require('@/assets/images/works1.jpg')
                    },
                    {
                        image:require('@/assets/images/works2.jpg')
                    },
                    {
                        image:require('@/assets/images/works3.jpg')
                    },
                    {
                        image:require('@/assets/images/works4.jpg')
                    },
                    {
                        image:require('@/assets/images/works5.jpg')
                    },
                    {
                        image:require('@/assets/images/works6.jpg')
                    },
                ],
                informations:[
                    {
                        date:'2020.XX.XX',
                        content:'デザイン雑誌「ＸＸＸＸＸＸ Vol.11』に掲載していただきました。'
                    },
                    {
                        date:'2020.XX.XX',
                        content:'ＸＸ月ＸＸ日から写真集「ＸＸＸＸＸＸＸ」の販売を開始します。'
                    },
                    {
                        date:'2019.XX.XX',
                        content:'【イベント開催のお知らせ】テキストテキストテキストテキストテキストテキストテキスト'
                    },
                    {
                        date:'2019.XX.XX',
                        content:'デザイン雑誌「ＸＸＸＸＸＸ Vol.10』に掲載していただきました。'
                    },
                    {
                        date:'2019.XX.XX',
                        content:'【個展開催のお知らせ】テキストテキストテキストテキストテキストテキストテキスト'
                    },
                ]
            }
        }
    }
</script>
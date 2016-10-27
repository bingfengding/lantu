<style lang="stylus" scoped rel="stylesheet/stylus">
    .news
        .container
            .news_bg
                background-image url("../images/news/bg.jpg")
                background-size cover
                height 650px
                position relative
                .news_bg_p1
                    position absolute
                    top 50%
                    left 10%
                .news_bg_p2
                    margin 0 auto
                    width 800px
                    padding-top 260px
                .news_bg_p3
                    position absolute
                    top 40%
                    right 10%
                .news_bg_p4
                    position absolute
                    bottom 10%
                    right 5%
        .news_main
            .title_list
                margin 0 auto
            .article_list
                position relative
                margin 30px auto
                width 45%
                min-width 850px
                padding-bottom 40px
                .page_c
                    position absolute
                    bottom 0
                    right 0
                    width 100%
                    height 22px
                    a
                        display block
                        float right
                        margin 0 5px
                        height 22px
                        padding 0 8px
                        font-size 12px
                        line-height 22px
                        border-radius 5px
                        background black
                        color rgb(240,240,240)


    *
        margin 0
</style>
<template>
    <div class="news">
        <div class="container">
            <div class="news_bg">
                <div class="news_bg_p1"><img src="../images/news/bg_p1.png" alt=""></div>
                <div class="news_bg_p2"><img src="../images/news/bg_p2.png" alt=""></div>
                <div class="news_bg_p3"><img src="../images/news/bg_p3.png" alt=""></div>
                <div class="news_bg_p4"><img src="../images/news/bg_p4.png" alt=""></div>
            </div>
        </div>
        <div class="news_main">
            <div class="title_list">
                <p>
                    <img src="../images/news/t_n.png">
                </p>
                <h1>经典案例</h1>
            </div>
            <div class="article_list">
                <div class="page_c">
                    <a class="last_pg">末页</a>
                    <a class="next_pg">下一页</a>
                    <div class="pg_num">

                    </div>
                    <a class="pre_pg">上一页</a>
                    <a class="first_pg">首页</a>
                </div>
            </div>
            <div class="pg_l_m">
                <div class="pg_l_img"><img :src="item.src"></div>
                <div class="pg_l_words" v-for="item of list">
                    <h1>{{headlines}}</h1>
                    <time>{{time}}</time>
                    <p>{{words}}</p>
                </div>
            </div>
        </div>


    </div>
</template>
<script>
    export default{
        data(){
            return{
                list:[
                    {
                        headlines:"兰途科技，运用企业号提供智慧校园解决方案",
                        time:"2016.08.22",
                        words:"据了解，由兰途科技筹建的北建移动门户微信企业号2.5.9已于近日正式上线。该企业号是基于智慧校园推出的微信第三方应用。根据学生反映，自北建移动门户上线以来，全校部分师生已经关注并绑定了此微信企业号...",
                         src:require("../images/news/ct8.png")
                    },
                    {
                        headlines:"兰途出品 | 中财移动门户上线！",
                        time:"2016.05.30",
                        words:"中财掌上校园正式开学了！兰途科技承建的中央财经大学官方移动门户正式上线，现已登陆苹果、安卓各大应用市场，在校师生可第一时间前往下载使用...",
                         src:require("../images/news/ct7.png")
                    }
                ]
            }
        },
        components:{

        }
    }
</script>

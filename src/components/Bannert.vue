<style lang="stylus" scoped rel="stylesheet/stylus">
    .bannert
        background-image url("../images/home/bg.png")
        background-size 100% 100%
        .ban_mobile
            overflow hidden
            width 1500px
            margin 0 auto
            ul
                position relative
                padding 80px 0
                width 4500px
                height 580px
                li
                    float left
                    width 300px
                    vertical-align top
                    transition all 0.5s

</style>
<template>
    <div class="bannert">
        <div class="title_list">
            <h2><img src="../images/home/t_c.png" alt=""></h2>
            <h1>经典案例</h1>
        </div>
        <div class="banner">
            <div class="ban_mobile">
            <ul>
                <li></li>
            </ul>

        </div>
            <div class="ban_page"></div>
            <div class="ban_nav"></div>
        </div>

    </div>
</template>
<script>
    export default{
        data(){
            return{

            }
        },
        components:{

        }
    }
</script>

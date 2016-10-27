<style lang="stylus" scoped rel="stylesheet/stylus">
    .header
        height 68px
        border-bottom 1px solid rgb(215,215,215)
        box-shadow 0 1px 2px rgb(208,208,208)
        background-color rgb(233,235,238)
        position fixed
        top 0
        width 100%
        z-index 999
        .w1100
            height 68px
            .logo
                float left
                height 68px
                padding-top 15px
                margin-right 80px
            ul
                float left
                li
                    float left
                    height 68px
                    line-height @height
                    text-align center
                    margin-left 80px
                    a
                        font-size 15px
                        &:hover
                            color rgb(167,195,30)


</style>
<template>
    <div class="header">
        <div class="w1100">
            <div class="logo">
                <img src="../images/currency/logo.png">
            </div>
            <ul>
                <li v-for="item of list" >
                    <router-link :to="item.href">{{item.name}}</router-link>
                </li>
            </ul>

        </div>
    </div>
</template>
<script>
    export default{
        data(){
            return{
                list : [
					{
						name : "首页",
						href : "/"
					},
					{
						name : "移动校园",
						href : "/mobilSchool"
					},
					{
						name : "经典案例",
						href : "/case"
					},
					{
						name : "公司动态",
						href : "/news"
					},
					{
						name : "招贤纳士",
						href : "/recruit"
					},
					{
						name : "联系我们",
						href : "/contact"
					}
				]
            }
        },
        components:{

        }
    }
</script>

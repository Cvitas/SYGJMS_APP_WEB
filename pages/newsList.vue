/**
* Created by cx on 2018/2/1.
* Include
* description 
*/
<template>
    <div class="wrap news-list-wrap">
        <div class="box">
            <div class="search-box">
                <div class="swiper-container search-items">
                    <div class="swiper-wrapper">
                        <div class="swiper-slide search-item active"><span>图片新闻</span></div>
                        <div class="swiper-slide search-item"><span>政策法规</span></div>
                        <div class="swiper-slide search-item"><span>大学生入伍</span></div>
                        <div class="swiper-slide search-item"><span>阳光政务</span></div>
                        <div class="swiper-slide search-item"><span>国防知识</span></div>
                    </div>
                </div>
            </div>
            <div class="box-scroll news-list-scroll" id="boxScrollChild">
                <div>
                    <div class="swiper-container swiper-top">
                        <div class="swiper-wrapper">
                            <div class="swiper-slide">
                                <div class="content-top news-2">
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="news-list-items">
                        <div class="news-list-item">
                            <div class="item-bg item-bg1"></div>
                            <div class="item-title">雪峰街道积极开展辖区重点优抚对象数据核查工作 </div>
                            <div class="item-time">2018-09-13</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg2"></div>
                            <div class="item-title">雪峰街道“三抓”提高住户记账质量</div>
                            <div class="item-time">2018-09-13</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg3"></div>
                            <div class="item-title">雪峰街道“四到位”扎实推进第四次全国经济普查工作</div>
                            <div class="item-time">2018-09-12</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg4"></div>
                            <div class="item-title">雪峰街道“四到位”扎实推进脱贫攻坚“秋季攻坚</div>
                            <div class="item-time">2018-09-10</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg5"></div>
                            <div class="item-title">雪峰街道开展秋季校园及周边食品安全大检查</div>
                            <div class="item-time">2018-09-05</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg5"></div>
                            <div class="item-title">雪峰街道开展秋季校园及周边食品安全大检查</div>
                            <div class="item-time">2018-09-05</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg5"></div>
                            <div class="item-title">雪峰街道全民健康生活方式日:“三减三健”促健康</div>
                            <div class="item-time">2018-09-03</div>
                        </div>
                        <div class="news-list-item">
                            <div class="item-bg item-bg5"></div>
                            <div class="item-title">雪峰街道“三全”做好“女儿节”期间各项综合治理工作</div>
                            <div class="item-time">2018-09-03 5</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    import iScroll from 'iScroll'
    import Swiper from 'swiper'
    export default {
        data() {
            return {
            }
        },
        mounted(){
            setTimeout(()=>{
                new Swiper ('.search-items', {
                    direction: 'horizontal',
                    slidesPerView:5,
                    loop: true,
                });
                new Swiper ('.swiper-top', {
                    direction: 'horizontal',
                    // 如果需要分页器
                    loop:true,
                });
                new iScroll('#boxScrollChild',{
                    probeType:2,
                    bounceTime: 250,
                    bounceEasing: 'quadratic',
                    mouseWheel:false,
                    scrollbars:false,
                    fadeScrollbars:true,
                    interactiveScrollbars:false,
                    preventDefault:false
                });
            },2000)
        },
        methods:{
        },
    }
</script>
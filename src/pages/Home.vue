<template>
    <div class="home">
        <searchs></searchs>
        <home-swiper></home-swiper>
        <number></number>
        <common></common>
        <home-footer></home-footer>
    </div>
</template>
<script>
import HomeFooter from "./components/footer"
import Searchs from "./components/search"
import HomeSwiper from "./components/swiper"
import Number from "./components/number"
import Common from "./components/common"
export default {
    name:'home',
    components:{
        HomeFooter,
        Searchs,
        HomeSwiper,Number,Common
    }
}
</script>
<style scoped>
.home{
    background-color: #eee;
}
</style>
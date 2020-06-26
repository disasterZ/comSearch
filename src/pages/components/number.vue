<template>
    <div class="number">
        <div class="num">
            <div>1314</div>
            <h1>注册企业</h1>
        </div>
        <div class="num">
            <div>1003</div>
            <h1>供应需求</h1>
        </div>
        <div class="num">
            <div>856</div>
            <h1>产品信息</h1>
        </div>
    </div>
</template>
<script>
export default {
    name:"number"
}
</script>
<style scoped>
.number{
    margin-top:3.2rem ;
    margin-bottom: 0.2rem;
    background-color: #fff;
    height: 1.4rem;
}
.num{
    width: 33%;
    height: 1.4rem;
    text-align: center;
    float: left;
    margin-bottom: 0.4rem;
}
.num div{
    color: #655cb9;
    font-size: 22px;
    margin: 0.2rem 0;
}
.num h1{
    font-size: 8px;
}
</style>
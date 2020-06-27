<template>
    <div class="search">
        <div class="head">
            <h1>订单开始</h1>
            <router-link to="/" tag="img"></router-link>
        </div>
        <div class="bd">
            <div class="name">
                <div class="inputs">
                    <div>项目名</div>
                    <input type="text" name="name" placeholder="项目名称">
                    <input type="text" name="func" placeholder="功能">
                    <input type="text" name="types" placeholder="类型">
                </div>
                <div class="result">
                    <div>智能匹配结果</div>
                    <div class="res">暂无</div>
                    <div>手动选择</div>
                    <div class="res">暂无</div>
                </div>
            </div>
            <div class="needs">
                <div>需求</div>
                <label>生产方<input type="radio" name="need" ></label>
                <label>设计师<input type="radio" name="need" ></label>
            </div>
            <div class="select">
                <div v-for="(list,index) of lists" :key="index">
                    {{list}}<input type="radio" name="select">
                </div>
            </div>
            <div class="info">
                <div>项目信息</div>
                <img>
            </div>
            <button id="sure">确认发布</button>
        </div>
    </div>
</template>
<script>
export default {
    name:"Search",
    data(){
        return{
            lists:["快速生产","区域范围","多厂合作","特殊精度","特殊工艺","工程验证"]
        }
    }
}
</script>
<style scoped>
.search{
    width: 100%;
    background-color: #eee;
}
.head{
    height: 2rem;
}
.head h1{
    padding-top: 0.8rem;
    padding-left: 0.5rem;
    font-size: 20px;
    font-weight: bold;
}
.head img{
    width: 0.8rem;
    height: 0.8rem;
    position:absolute;
    right: 0.4rem;
    top: 0.5rem;
}
.bd{
    border-top-left-radius: 0.5rem;
    border-top-right-radius:0.5rem;
    width: 100%;
}
.name{
    height: 3.2rem;
    background-color: #fff;
    border-top-left-radius: 0.5rem;
    border-top-right-radius:0.5rem ;
}
.needs{
    margin-top: 0.2rem;
    background-color: #fff;
    height: 1.5rem;
}
.select{
    margin-top: 0.2rem;
    background-color: #fff;
    height: 2rem;
}
.info{
    margin-top: 0.2rem;
    background-color: #fff;
    height: 5rem;
}
.inputs{
    width: 100%;
    display: inline-block;
    margin: 0.6rem 0.4rem;
}
.inputs div{
    display: inline-block;
    font-size: 20px;
    height: 0.5rem;
    vertical-align: middle;
}
.inputs input{
    width: 24%;
    background-color:#ddd ;
    height: 0.5rem;
}
.result{
    width:100%;
    margin: 0.6rem;
}
.res{
    width: 1.5rem;
    background-color: #ccc;
    color:#ccc;
}
.result div{
    display: inline-block;
    font-size: 16px;
}
.needs div{
    display: inline-block;
    margin: 0.6rem 0.4rem;
    font-size: 20px;
}
.needs label{
    margin:0 0.6rem
}
.needs label input{
    margin: 0 0.2rem;
}
.select div{
    display: inline-block;
    width: 28%;
    margin-top: 0.3rem;
    margin-left:0.3rem ;
    height: 0.5rem;
    text-align: center;

}
.select div input{
    margin-left: 0.1rem;
}
.info div{
    padding: 0.3rem 0.4rem;
    font-size: 20px;
}
.info img{
    width: 6.5rem;
    height: 4rem;
    background-color: #ccc;
    margin:0rem 0.4rem;
}
#sure{
    width: 25%;
    height: 0.6rem;
    background-color: green;
    position: fixed;
    bottom: 0.8rem;
    left: 35%;
    color: #fff;
    background-color: #416dcb;
    border-radius: 0.2rem;
}
</style>
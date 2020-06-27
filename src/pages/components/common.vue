<template>
    <div class="common">
        <div class="head">
            <div class="more">更多></div>
            <div class="title">共享大厅</div>
        </div>
        <div class="icon" v-for="(icon,index) of icons" :key="index">
            <img>
            <p>{{icon.name}}</p>
        </div>
    </div>
</template>
<script>
export default {
    name:"Common",
    data(){
        return{
            icons:{
                "1":{
                    url:"",
                    name:"产能"
                },
                "2":{
                    url:"",
                    name:"仓储"
                },
                "3":{
                    url:"",
                    name:"设备"
                },
                "4":{
                    url:"",
                    name:"生产线"
                },
                "5":{
                    url:"",
                    name:"人才"
                },
                "6":{
                    url:"",
                    name:"采购"
                },
                "7":{
                    url:"",
                    name:"技术"
                },
                "8":{
                    url:"",
                    name:"综合"
                }
            }
        }
    }
    
}
</script>
<style scoped>
@import '../../assets/style/head.css';
.common{
    background-color: #fff;
    height: 4rem;
    padding-bottom: 0.2rem;
}
.icon{
    width: 25%;
    text-align: center;
    margin-top: 0.2rem;
    float: left;
}
.icon img{
    background-color: #ddd;
    width: 0.7rem;
    height: 0.7rem;
    border-radius: 0.2rem;
    
}
.icon p{
    font-size: 6px;
    margin-top: 0.2rem;
}
</style>
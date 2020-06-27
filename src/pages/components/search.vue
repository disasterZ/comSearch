<template>
    <div class="sh">
        <router-link class="input" tag="div" to="/search">
            <div class="btn">

            </div>
        </router-link>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.sh{
    width: 100%;
    height: 1rem;
    padding-top:0.2rem;

}
.input{
    width: 80%;
    height: .7rem;
    background-color: #fff;
    margin:0 auto;
    border:1px solid #1062c5;
    border-radius: 20px;
}
.btn{
    width: 20%;
    height: 100%;
    background-color: #1062c5;
    border-radius: 20px;
    float: right;
}
</style>
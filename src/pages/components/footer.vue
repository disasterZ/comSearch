<template>
  <div class="footer">
    <div class="icon">
      <div class="ficon">
        <img/>
        <h5>首页</h5>
      </div>
      <div class="ficon">
        <img/>
        <h5>企业库</h5>
      </div>
      <div class="ficon">
        <div class="main">
          <img/>
          <h1>发布</h1>
        </div>
      </div>
      <div class="ficon">
        <img/>
        <h5>管理</h5>
      </div>
      <div class="ficon">
        <img/>
        <h5>我的</h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {};
  },
  props: {
    city: String
  }
};
</script>

<style scoped>
.footer{
  position: fixed;
  bottom: 0px;
  background-color: red;
  width: 100%;
  box-shadow:1px -1px #eee;
}
.icon{
  display: flex;
  line-height: 1rem;
  width: 100%;
  background-color:#fff;
  margin: 0 auto;
  text-align: center;
}
.ficon{
  width: 15%;
  margin: 0 .2rem;
  padding-bottom: 0.1rem;
  line-height: 0.3rem; 
}
.ficon img{
  width: 0.6rem;
  height: 0.5rem;
  padding:0.2rem;
}
.ficon h5{
  font-size: 10px;
}
.main{
  position: absolute;
  bottom: 0;
}
.main img{
  width: 1.1rem;
  height: 1.2rem;
  padding:0.2rem;
}

</style>

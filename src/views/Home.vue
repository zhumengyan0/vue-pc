<template>
  <div class="home">
    <!-- 轮播图/走马灯 -->
    <el-carousel :interval="4000" type="card" height="200px">
      <el-carousel-item v-for="item in imgs" :key="item">
        <h3 class="medium">
          <img :src="item" alt="">
        </h3>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default{
  data () {
    return {
      imgs: [
        "https://dss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=598069525,3705173246&fm=5",
        "https://dss0.baidu.com/6ONWsjip0QIZ8tyhnq/it/u=942120003,4005302423&fm=5",
        "https://dss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=2300875363,445064071&fm=5",
        "https://dss1.baidu.com/6ONXsjip0QIZ8tyhnq/it/u=620185774,165030302&fm=5",
        "https://dss1.bdstatic.com/70cFuXSh_Q1YnxGkpoWK1HF6hhy/it/u=2659231633,3003203990&fm=26&gp=0.jpg",
        "https://dss3.bdstatic.com/70cFv8Sh_Q1YnxGkpoWK1HF6hhy/it/u=3344241222,2470179097&fm=26&gp=0.jpg"
      ]
    }
  }
}
</script>
<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
  img{
    width: 366px!important;
    height: 166px!important;
  }
</style>

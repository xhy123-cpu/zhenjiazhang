<template>
<main>
    <div class="top-show">
        <img src="../../../public/service-img/T_6OQGB9OT_t1.jpg" alt="">
        <img src="../../../public/service-img/u=3869183228,3821620769&fm=253&fmt=auto&app=138&f=JPEG.jpg" alt="">
        <img src="../../../public/service-img/53.png" alt="">
        <img src="../../../public/service-img/55.png" alt="">
        <img src="../../../public/service-img/56.png" alt="">
        <img src="../../../public/service-img/57.png" alt="">
    </div>
    <div class="showbar" @click="make">财税订单填写</div>
    <div class="gongsituijian">公司推荐</div>
    <div class="bottom-show">
        <div><img src="../../../public/service-img/1.png" alt=""><img src="../../../public/service-img/2.png" alt=""><img src="../../../public/service-img/3.png" alt=""></div>
        <div><img src="../../../public/service-img/4.png" alt=""><img src="../../../public/service-img/5.png" alt=""><img src="../../../public/service-img/6.png" alt=""></div>
        <div><img src="../../../public/service-img/7.png" alt=""><img src="../../../public/service-img/8.png" alt=""><img src="../../../public/service-img/9.png" alt=""></div>
    </div>
    <div class="footer">
    <div class="grid-content ep-bg-purple"></div>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">公司简介</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">平台服务</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">隐私与帮助</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">关于我们</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">财会学习</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">协议与规则</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">公司介绍</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">财税服务</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">隐私政策</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">管理团队</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">打假举报</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">防骗指南</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">公司文化</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">职位招聘</div></el-col>
      <el-col :span="4"><div class="grid-content ep-bg-purple">使用帮助</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">加入我们</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="4"><div class="grid-content ep-bg-purple">联系我们</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="12"><div class="grid-content ep-bg-purple"></div></el-col>
      <el-col :span="12"><div class="grid-content ep-bg-purple">公司地址：安徽省合肥市合肥工业大学</div></el-col>
    </el-row>
  </div> 
</main>
</template>

<script>
export default {
    emits:['order'],
    methods:{
        make(){
            if(this.$emit('order','Order'))
            console.log('ok');
        }
    }
}
</script>

<style lang="less">
// @import '../../less/Service.less'
.top-show{
  margin-left: 150px;
  margin-right: 150px;
  height: 420px;
  position: relative;
  img{
      position: absolute;
      width: 240px;
      &:nth-child(1){
      height: 420px;
      left: 0;
      }
      &:nth-child(2){
      height: 420px;
      width: 240px;
      left: 240px;
      }
      &:nth-child(3){
      height: 210px;
      left: 480px;
      }
      &:nth-child(4){
      height: 210px;
      left: 720px;
      bottom: 0;
      }
      &:nth-child(5){
      height: 210px;
      left: 480px;
      bottom: 0;
      }
      &:nth-child(6){
      height: 210px;
      left: 720px;
      }
  }

}
.gongsituijian{
    font-size: larger;
    height: 50px;
    font-weight: 450;
    margin: 20px 188px;
    border-bottom: 1px solid #000;
}
.bottom-show{
    margin-left: 210px;
    margin-right: 210px;
    height: 840px;
    >div{
        margin-top: 20px;
        display: flex;
        justify-content: space-between;
        height: 260px;
        img{
            border-radius: 10px;
        }
    }
}
</style>
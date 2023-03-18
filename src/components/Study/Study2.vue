<template>
  <main>
    <div class="showbar">法律法规指导区</div>
    <div class="box-s2">
        <img src="../../../public/study-img/法律法规精彩内容.png">
    </div>
    <div class="text">最新法律解读</div>
    <div class="box-s2">
        <ul>
            <li>财政部解读《会计改革与发展“十三五”规划纲要》</li>
            <li>名师专家带你解读”金税四期”系列</li>
            <li>解读《财政总会计制度》</li>
            <li>关于电子烟消费税征收管理有关事项公告解读</li>
            <li>企业投入基础研究税收优惠政策操作指南解读</li>
            <li>工业和信息化部关于延续新能源汽车免征车辆购置税政策解读</li>
            <li>养老金有关所得税政策解读</li>
            <li>增值税纸质专用发票防伪措施有关事项解读 </li>
            <li>优化若干税收征管服务事项解读</li>
            <li>关于中国人民共和国进出口税着公告解读</li>
            <li>关于延续实施有关个人所得税优惠政策公告解读</li>
            <li>《国家艺术基金财务管理办法》解读</li>
        </ul>
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
  name:'Study2'

}
</script>

<style lang="less">
.box-s2{
    margin: 20px 188px;
    border: 2px solid #000;
    height: 500px;
    overflow-y: scroll;
    img{
        width: 100%;
    }

}
.text{
    height: 70px;
    line-height: 70px;
    font-size: 40px;
    font-weight: bold;
}

</style>
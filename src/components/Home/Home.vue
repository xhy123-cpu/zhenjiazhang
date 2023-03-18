<script lang="ts" setup>
import { ref } from 'vue'

import {
    User,
    Setting,
    Search
} from '@element-plus/icons-vue'



</script>

<template>
<div>
  <main>

  <div class="box">
    <div class="info-left">
      <ul>
        <li>代理记账资格行政审批有哪...</li>
        <li>申请代理记账资格应具...</li>
        <li>申请代理记账许可证书...</li>
        <li>代理记账机构年度备案...</li>
        <li>小微企业与代理记账...</li>
        <li>代理记账机构年度检查问题...</li>
        <li>会计考试报名条件...</li>
        <li>会计人员继续教育问题...</li>
        <li>会计专业技术证书从哪里领取...</li>
      </ul>
    </div>
    <div class="info-right">
      <!-- 轮播图 -->
        <div class="block text-center">
          <el-carousel height="280px">
            <el-carousel-item v-for="item in 4" :key="item">
              <img src="../../../public/home-img/a.jpg" style="height: 280px;width: 100%;" v-if="item===1">
              <img src="../../../public/home-img/b.jpg" style="height: 280px;width: 100%;" v-if="item===2">
              <img src="../../../public/home-img/c.jpg" style="height: 280px;width: 100%;" v-if="item===3">
              <img src="../../../public/home-img/d.jpg" style="height: 280px;width: 100%;" v-if="item===4">
            </el-carousel-item>
          </el-carousel>
        </div>
        <img src="../../../public/home-img/e.png" alt="" style="height: 135px;width: 100%; margin-top: 10px;">
    </div>
  </div>
  <div class="bankuai" style="background-color: #e3f1fa;">
    <div class="bankuai-child">
      <img src="../../../public/home-img/47.png" alt="" class="bankuai-img">
      <div class="bankuai-text">学习天地</div>
    </div>
    <div class="bankuai-child">
      <img src="../../../public/home-img/49.png" alt="" class="bankuai-img">
      <div class="bankuai-text">财税业务</div>
    </div>
    <div class="bankuai-child">
      <img src="../../../public/home-img/52.png" alt="" class="bankuai-img">
      <div class="bankuai-text">财企汇聚</div>
    </div>
    <div class="bankuai-child">
      <img src="../../../public/home-img/51.png" alt="" class="bankuai-img">
      <div class="bankuai-text">打假举报</div>
    </div>
  </div>
  <!-- 显示区 -->
  <div class="xianshiqu">

  </div>
  <!-- 底部 -->
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

</div>
</template>





<style lang="less">
@import '../../less/Home.less';

</style>>







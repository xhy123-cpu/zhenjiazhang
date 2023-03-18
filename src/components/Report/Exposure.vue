<template>
  <main>
    <div class="showbar" @click="dajia">假账曝光平台</div>
    <div class="zhongdazuojia">重大作假案例曝光</div>
    <div class="select-report-ex">
        <div>
            <div><div>宜华生活:信息披露违法违规案</div></div>
            <div><div>广州浪奇:信息披露违法违规案</div></div>
        </div>
        <div>
            <div><div>龙力生物:信息披露违法违规案</div></div>
            <div><div>亚太药业:信息披露违法违规案</div></div>
        </div>
    </div>
    <div class="zhongdazuojia">平台检举成功案例</div>
    <div class="select-report-ex" style="margin-bottom: 300px;">
        <div>
            <div><div>xxx企业:信息披露违法违规案</div></div>
            <div><div>xxx企业:信息披露违法违规案</div></div>
        </div>
        <div>
            <div><div>xxx企业:信息披露违法违规案</div></div>
            <div><div>xxx企业:信息披露违法违规案</div></div>
        </div>
        <div>
            <div><div>xxx企业:信息披露违法违规案</div></div>
            <div><div>xxx企业:信息披露违法违规案</div></div>
        </div>
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

}
</script>

<style lang="less">
.zhongdazuojia{
    font-size: 30px;
    height: 50px;
    font-weight: 450;
    margin-top: 40px;
    margin-left: 188px;
    margin-right: 188px;
    border-bottom: 1px solid #000;
    line-height: 50px;

}
.select-report-ex{
    margin: 20px 300px;
    height: 500px;
    >div{
        height: 240px;
        margin-bottom: 10px;
        border-radius: 10px; 
        >div{
            height: 240px;
            margin-right: 10px;
            width: 300px;
            background-color: #79bee8;
            display: inline-block;
            position: relative;
            border-radius: 10px;
            transition: 0.3s linear;
            &:hover{
              background-color: #22ee96;
            }
            font-size: 40px;

        }
    }
}
</style>
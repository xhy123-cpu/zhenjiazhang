<template>
  <main>
    <div class="show-login">
        <div class="title-login">用户账号注册</div>
        <input type="text" class="text-login" placeholder="手机号">
        <div class="verify-login">
          <input type="text" class="text-login" placeholder="验证码">
          <div>获取验证码</div>
        </div>
        <input type="password" class="text-login" placeholder="密码设置">
        <input type="password" class="text-login" placeholder="确认密码">
        <div class="rule-login">
            <input type="checkbox" style="background-color:#d1cfcf;" v-model="canUse">阅读并同意甄假账的服务协议和个人信息保护政策
        </div>
        <button class="btn-login" :disabled="!canUse">注册</button>
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
    data() {
        return {
            canUse: false,
        }
    },
}
</script>

<style lang="less">
.verify-login{
    height: 40px;
    line-height: 40px;
    font-size: 30px;
    margin-bottom: 20px;
    >input{
        vertical-align: 1px;
        width: 150px;
        border:1px solid #000;
    }
    >div{
        font-size: 20px;
        vertical-align: 1px;
        display: inline-block;
        width: 150px;
        height: 43px;
        color: #d3cccc;
        background-color: #cfe8f8;
        &:hover{
            cursor: pointer;
            color: rgb(219, 135, 24);
        }
    }
        
}

</style>
<template>
  <main>
    <div class="show-login">
        <div class="title-login">用户账号登陆</div>
        <input type="text" class="text-login" placeholder="账号" v-model="myname">
        <input type="password" class="text-login" placeholder="密码" v-model="mypass">
        <div class="rule-login">
            <input type="checkbox" style="background-color:#d1cfcf;" v-model="canUse">阅读并同意甄假账的服务协议和个人信息保护政策
        </div>
        <button class="btn-login" :disabled="!canUse" @click="log">登录</button>
        <div class="link-login">
            <a href="#" @click="make">未有账号，点击注册</a>
            <a href="#">忘记密码</a>
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
data() {
    return {
        canUse: false,
        admin: 'admin',
        password: '1314520',
        myname: '',
        mypass:''
    }
},
emits: ['report'],
methods: {
    make() {
        if(this.$emit('report','Register'))
        console.log('ok');
    },
    log() {
        if (this.admin==this.myname&&this.mypass) {
        this.$emit('report','Person')
        
        }
        else {
            window.alert('密码或账号错误，请重新输入')
            console.log(111);
        }
    }
    }
}
</script>

<style lang="less">
.show-login{
    background-color: #fff;
    margin-left: 350px;
    margin-right: 350px;
    height: 500px;
    padding-top: 1px;
    border-radius: 20px;
    .title-login{
        height: 40px;
        line-height: 40px;
        font-size: 30px;
        margin-top: 30px;
        
    }
}
.text-login{
    height: 30px;
    width: 300px;
    font-size: 20px;
    font-weight: lighter;
    padding-left: 4px;
    padding-top: 4px;
    padding-bottom: 4px;
    margin-top: 15px;
}
.rule-login{
    margin-top: 15px;
    color: #d1cfcf;
}
.btn-login{
    background-color: #78b3f8;
    display: inline-block;
    margin-top: 30px;
    height: 50px;
    line-height: 50px;
    width: 350px;
    font-size: 30px;
    border-color: #78b3f8;
    border-radius: 15%;
    cursor: pointer;
    &:disabled{
        cursor: not-allowed;
    }
}
.link-login{
    margin:30px 20px ;
    display: flex;
    justify-content: space-between;
}
</style>
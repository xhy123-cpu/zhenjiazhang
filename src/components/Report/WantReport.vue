<template>
  <main>
    <div class="showbar">举报平台</div>
    <div class="zhongdazuojia">网络举报须知</div>
    <div class="xuzhi" style="height: 40px;"> 1.每位用户只能注册一个账户。<br />
2.没有违反法律法规的具体事实和证据，请勿随意举报。<br />
3.同一违法行为，没有新的事实和证据，请勿重复举报。<br />
4.禁止使用谩骂、辱骂、人身攻击等不文明用语。<br />
5.平台审核需要一定的时间，请耐心等待，平台将尽快给予答复和协助。<br />
    </div>
    <input type="checkbox" v-model="canUse">我已阅读并同意以上内容<br/>
    <button :disabled="!canUse" class="jubao-want" @click="tianxie">举报填写</button>
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
            canUse:false
        }
    },
    emits:['report'],
    methods: {
      tianxie() {
        if(this.$emit('report','WillReport'))
        console.log('ok');
    }
    }
}
</script>

<style lang="less">
.jubao-want{
    margin-top: 30px;
    font-size: 20px;
    background-color: #79bee8;
    border: 0.5px solid #79bee8;
    border-radius: 5px;
    cursor: pointer;
    &:disabled{
        cursor: not-allowed;
    }
}
</style>
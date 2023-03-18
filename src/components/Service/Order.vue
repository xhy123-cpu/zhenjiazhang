<template>
    <main>
        <div class="showbar">订单填写</div>
        <div class="xianshihang" v-for='(item,index) in case' :key="index">
            <span class="mingcheng">{{ item }}:</span>
            <input type="text" class="order-input">
        </div>
        <div class="xianshihang">
            <span class="mingcheng">行业信息:</span>
            <input type="text" placeholder="电子商务、科技、贸易等" class="order-input">
        </div>
        <div class="xianshihang">
            <span class="mingcheng">价格意愿:</span>
            <input type="text" placeholder="可接受的价格范围" class="order-input">
        </div>
        <div class="xianshihang" style="height: 170px;">
            <span class="mingcheng">公司主要业务:</span>
            <textarea placeholder="公司交易类型、简述一下公司主要经营活动" class="gs" cols="30" rows="10"></textarea>
        </div>
        <div class="xianshihang">
            <span class="mingcheng">业务需求:</span>
            <input type="text" placeholder="代理记账、汇算清缴、审计报告等" class="order-input">
        </div>
        <div class="xianshihang">
            <span class="mingcheng">备注:</span>
            <input type="text" placeholder="可接受的价格范围" class="order-input">
        </div>
        <div style="height: 60px;"></div>
        <span class="sub" @click="make">提交</span>
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
    data(){
        return{
            case:['经济体名称','账号','联系方式','地址','法人姓名','身份证号','期望合作年限','年收入']
        }
    },
    emits:['service'],
    methods:{
        make(){
            if(this.$emit('service','Service'))
            console.log('ok');
        }
    }
}
</script>

<style lang="less">
.order-input{
    height: 20px;
    width: 400px;
    border: 1.5px solid #000;
    background-color: #dcebf4;
    position: absolute;
    right: 384px;
    top: 5px;
}
.mingcheng{
    height: 30px;
    font-size: larger;
    line-height: 30px;
    font-weight: bold;
    position: absolute;
    right: 800px;
}
.xianshihang{
    height: 50px;
    position: relative;
}
.gs{
    width: 400px;display: inline-block;
    position: absolute;font-size:medium;right: 384px;
    background: #dcebf4;
    border: 1.5px solid #000;
}
.sub{
    height: 100px;color: #fff;background-color: #4b81bf;
    font-size: 40px; padding: 6px 15px;border-radius: 10px;margin-top: 70px;
    cursor: pointer;
    &:hover{
        color: brown;
        border: 1px solid #ce7e2f;
    }

}
</style>
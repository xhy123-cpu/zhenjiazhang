<template>
  <main>
    <div class="select-report">
        <div>
            <div>
                <img src="../../../public/report-img/46.png">
                <div>我要投诉&nbsp;></div>
            </div>
            <div @click="jubao">
                <img src="../../../public/report-img/47.png">
                <div>我要举报&nbsp;></div>
            </div>
        </div>
        <div>
            <div>
                <img src="../../../public/report-img/48.png">
                <div>我要咨询&nbsp;></div>
            </div>
            <div>
                <img src="../../../public/report-img/49.png">
                <div>我要建议&nbsp;></div>
            </div>
        </div>
    </div>
    <div class="showbar" @click="dajia">假账曝光平台&nbsp;>&nbsp;>&nbsp;></div>
    <div class="pingtaixuzhi">平台须知</div>
    <div class="xuzhi"> 欢迎您进入举报服务平台，您可根据自身诉求类别，通过相应的栏目进行提交诉求
本平台接受四类诉求事项：<br />
1. 投诉事项，即平台用户反映在购买平台产品或接受相关服务时，与平台合作商及平台服务人员发生纠纷的。<br />
2. 举报事项，即任何单位和个人举报涉嫌偷税漏税、虚增收入等财务做假违规行为，请求平台予以向国家相关部门进行检举的协助服务的 。<br />
3.咨询事项，即举报者对假账举报流程或财税服务相关事项提出咨询的。<br />4. 意见建议事项，即平台用户对平台服务或协助打假工作提出意见建议的。 
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
  emits:['report'],
  methods: {
    dajia(){
      if(this.$emit('report','Exposure'))
      console.log('ok');
    },
    jubao() {
      if(this.$emit('report','WantReport'))
      console.log('ok');
    }
  }
    
}
</script>

<style lang="less">
.select-report{
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
            background-color: #ffffff;
            display: inline-block;
            position: relative;
            border-radius: 10px;
            transition: 0.3s linear;
            &:hover{
                cursor: pointer;
                background-color: #56f2e1;
            }
            >div{
                height: 60px;
                font-size: 30px;
                position: absolute;
                top: 20px;
                left: 80px;
                color: #4b81bf;
                
            }
            img{
                position: absolute;
                left: 10px;
                top: 10px;
                height: 60px;
            }
        }
    }
}
.pingtaixuzhi{

    font-size: 40px;
    font-weight: bold;
    height: 50px;
    font-weight: 450;
    margin-left:  220px;
    margin-right:  220px;
    margin-top: 100px;
    border-bottom: 1px solid #000;
}
.xuzhi{
    margin: 20px 188px 188px;
    text-align: left;
    font-size: larger;
    

}
</style>
<template>
    <main>
      <div class="showbar">个性化学习区</div>
      <div class="box">
      <div class="info-left-s4">
        <div class="active" @click="read(1)">假账甄别学习</div>
        <div class="" @click="read(2)">就业经验分享</div>
        <div class="" @click="read(3)">财务分析学习</div>
        <div class="" @click="read(4)">智能税务分析</div>
        <div class="" @click="read(5)">假账举报学习</div>
      </div>
      <div class="info-right-s4">
        <img src="../../../public/home-img/1.png">
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
      name:"Study1",
      methods:{
          read:function(id){
              document.querySelector('.active').className=''
  
              
              document.querySelectorAll('.info-left-s4 div')[id-1].className='active'
              document.querySelector('img').src=`../../../public/study-img/study4//${id}.png`
          }
      }
  }
  </script>
<style lang="less">
.showbar{
    background-color: #4b81bf;
    height: 75px;
    border-radius: 20px;
    margin: 20px 188px;
    font-size: 50px;
    line-height: 75px;
    font-weight: bold;
    color: #fff;
}
.info-left-s4{
font-size: 30px ;
position: absolute;
height: 100%;
width: 30%;


div{
  margin: 15px;
  border-radius: 10px;
  background-color: #fff;  
  cursor: pointer;  
}
.active{
    background-color: #4b81bf;
}
}
.info-right-s4{
position: absolute;
right: 0;
height: 100%;
width: 62%;
// border: 1.5px solid #000;
overflow-y: scroll;
img{
    width: 100%;
}


}
</style>
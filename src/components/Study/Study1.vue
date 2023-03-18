<template>
  <main>
    <div class="showbar">小白学习讨论区</div>
    <div class="box">
    <div class="info-left-s1">
      <div class="active" @click="read(1)">会计实操</div>
      <div class="" @click="read(2)">财务软件学习</div>
      <div class="" @click="read(3)">财务岗位学习</div>
      <div class="" @click="read(4)">基础知识刷题</div>
    </div>
    <div class="info-right-s1">
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

            
            document.querySelectorAll('.info-left-s1 div')[id-1].className='active'
            document.querySelector('img').src=`../../../public/home-img/${id}.png`
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
        cursor: pointer;
        &:hover{
          color: brown;
          border: 1px solid #fbca06;
        }
    }
  .info-left-s1{
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
  .info-right-s1{
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
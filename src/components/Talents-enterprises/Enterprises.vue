<template>
    <main>
        <div class="top-show">
            <img src="../../../public/service-img/T_6OQGB9OT_t1.jpg">
            <img src="../../../public/service-img/u=3869183228,3821620769&fm=253&fmt=auto&app=138&f=JPEG.jpg">
            <img src="../../../public/enterprises-img/top-img/1.png">
            <img src="../../../public/enterprises-img/top-img/2.jpeg">
            <img src="../../../public/enterprises-img/top-img/3.jpeg">
            <img src="../../../public/enterprises-img/top-img/4.jpg">
        </div>
        <div class="title">实习生推荐</div>
        <div class="info-bar">
          <div class="info-child" v-for="item in items1" :key="item">
            <span>{{ item }}</span>
            <div></div>
          </div>
        </div>
        <div class="bottom-show">
            <div><img src="../../../public/enterprises-img/shixisheng-img/3.png"><img src="../../../public/enterprises-img/shixisheng-img/4.png"><img src="../../../public/enterprises-img/shixisheng-img/5.png"></div>
            <div><img src="../../../public/enterprises-img/shixisheng-img/2.png"><img src="../../../public/enterprises-img/shixisheng-img/3.png"><img src="../../../public/enterprises-img/shixisheng-img/4.png"></div>
            <div><img src="../../../public/enterprises-img/shixisheng-img/5.png"><img src="../../../public/enterprises-img/shixisheng-img/1.png"><img src="../../../public/enterprises-img/shixisheng-img/2.png"></div>
        </div>
        <div class="title" style="margin-top: 100px;">财务人员推荐</div>
        <div class="info-bar">
          <div class="info-child" v-for="item in items2" :key="item">
            <span>{{ item }}</span>
            <div></div>
          </div>
        </div>
        <div class="bottom-show">
            <div><img src="../../../public/enterprises-img/shixisheng-img/3.png"><img src="../../../public/enterprises-img/shixisheng-img/4.png"><img src="../../../public/enterprises-img/shixisheng-img/5.png"></div>
            <div><img src="../../../public/enterprises-img/shixisheng-img/2.png"><img src="../../../public/enterprises-img/shixisheng-img/3.png"><img src="../../../public/enterprises-img/shixisheng-img/4.png"></div>
            <div><img src="../../../public/enterprises-img/shixisheng-img/5.png"><img src="../../../public/enterprises-img/shixisheng-img/1.png"><img src="../../../public/enterprises-img/shixisheng-img/2.png"></div>
        </div>
        <div class="title">城市推荐</div>
        <div class="city">
          <div><img src="../../../public/enterprises-img/city-img/49.png">
            <img src="../../../public/enterprises-img/city-img/50.png">
            <img src="../../../public/enterprises-img/city-img/51.png">
            <img src="../../../public/enterprises-img/city-img/52.png">
            <img src="../../../public/enterprises-img/city-img/53.png">
          </div>
          <div><img src="../../../public/enterprises-img/city-img/54.png">
            <img src="../../../public/enterprises-img/city-img/55.png">
            <img src="../../../public/enterprises-img/city-img/56.png">
            <img src="../../../public/enterprises-img/city-img/57.png">
            <img src="../../../public/enterprises-img/city-img/58.png"></div>
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
        emits:['order'],
        methods:{
            make(){
                if(this.$emit('order','Order'))
                console.log('ok');
            }
        },
      data(){
        return{
          items1:[
          '职位','距离','薪资','学历','规模','岗位'
        ],
          items2:[
          '职位','经验','薪资','学历','规模','岗位'
        ]}
      }
    }
    </script>
    
    <style lang="less">
    .city{
    margin-left: 210px;
    margin-right: 210px;
    height: 200px;
    >div{
      display: flex;
      justify-content: center;
      img{
        height: 100px;
        width: 180px;
      }
    }
    }
    .top-show{
        margin-left: 150px;
        margin-right: 150px;
        height: 420px;
        position: relative;
        img{
            position: absolute;
            width: 240px;
            &:nth-child(1){
            height: 420px;
            left: 0;
            }
            &:nth-child(2){
            height: 420px;
            width: 240px;
            left: 240px;
            }
            &:nth-child(3){
            height: 210px;
            left: 480px;
            }
            &:nth-child(4){
            height: 210px;
            left: 720px;
            bottom: 0;
            }
            &:nth-child(5){
            height: 210px;
            left: 480px;
            bottom: 0;
            }
            &:nth-child(6){
            height: 210px;
            left: 720px;
            }
        }
    
    }
    .gongsituijian{
        font-size: larger;
        height: 50px;
        font-weight: 450;
        margin: 20px 188px;
        border-bottom: 1px solid #000;
    }
    .bottom-show{
        margin-left: 210px;
        margin-right: 210px;
        height: 840px;
        >div{
            margin-top: 20px;
            display: flex;
            justify-content: space-between;
            height: 260px;
            img{
                border-radius: 10px;
            }
        }
    }
    .title{
      height: 50px;
      font-size: 40px;
      line-height: 50px;
      font-weight: bolder;
      margin-top: 50px;
    }
    .info-bar{
      margin-left: 210px;
      margin-right: 210px;
      height: 40px;
      display: flex;
      justify-content: space-around;
      border-bottom: 1px solid #000;
    }
    .info-child{
      font-weight: bolder;
      font-size: large;
      line-height: 40px;
      height: 40px;
      position: relative;
      display: inline-block;
      span{
        line-height: 40px;
        height: 40px;
        display: inline-block;
      }
      div{
        position: absolute;
        top: 18px;
        margin-left: 2px;
        display: inline-block;
        width: 0;
        border-top: 10px solid #000;
        border-bottom: 10px solid transparent;
        border-left: 10px solid transparent;
        border-right: 10px solid transparent;
      }
    }

    </style>
<template>
  <main>
    <div class="showbar">疑难杂症答疑区</div>
    <div class="box" style="height: 800px;">
    <div class="info-left-s1">
      <div class="active" @click="read(1)">实操答疑</div>
      <div class="" @click="read(2)">法律法规答疑</div>
      <div class="" @click="read(3)">软件学习答疑</div>
      <div class="" @click="read(4)">假账甄别答疑</div>
    </div>
    <div class="info-right-s3">
      <div class="jingxuan"><img src="../../../public/study-img/1.png" alt=""></div>
      <component :is="comName" :myDiscuss="myDiscuss[index]"></component>
        <div>
            <textarea name="" id="" cols="30" rows="10" placeholder="我来说说" ref="text"></textarea>
            <div @click="send">发送</div>
        </div>
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
import One from './Study3/One.vue'
import Two from './Study3/Two.vue'
import Three from './Study3/Three.vue'
import Four from './Study3/Four.vue'

export default {
    methods:{
        read(id){
            this.index=id-1
            document.querySelector('.active').className=''
            document.querySelectorAll('.info-left-s1 div')[id-1].className='active'
            document.querySelector('img').src=`../../../public/home-img/${id}.png`
            this.comName=this.myCom[id-1]

        },
        send(){
            this.myDiscuss[this.index].push(this.$refs.text.value)
            this.$refs.text.value=''
        }
    },
    data(){
        return{
            comName:'One',
            myCom:['One','Two','Three','Four'],
            index:0,
            myDiscuss:[
                [],[],[],[]
            ]
        }
        
    },
    components:{One,Two,Three,Four}
}
</script>

<style lang="less">
.info-right-s3{
    position: absolute;
    right: 0;
    height: 100%;
    width: 62%;
    // border: 1.5px solid #000;


    
}
.jingxuan{
    height: 200px;
    overflow-y: scroll;
    border-bottom: 1px dashed #000;
    >img{
        width: 100%;
    }
}
.taolun{
    height: 450px; background-color:aliceblue ;
}

textarea{
    resize: none;
    height: 150px;
    width: 100%;
    overflow-y: scroll;
    position: relative;
    font-size: 40px;
    ~div{
        background-color: #0ca7f7;
        position: absolute;
        bottom: 5px;
        right: 30px;
        height: 30px;
        width: 60px;
        z-index: 99;
        border-radius:4px ;
        line-height: 30px;
        font-weight: bold;
        cursor: pointer;
    }
}
.suhongling{
  li{
    font-size: medium;
  }
}
</style>
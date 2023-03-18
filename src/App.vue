<template>
  <div style="background-color: #cfe8f8;">
  <!--导航栏  -->
  <el-menu
    style="position: fixed;top: 0px;width: 100vw;z-index: 999;"
    :default-active="activeIndex2"
    class="el-menu-demo"
    mode="horizontal"
    background-color="#4b81bf"
    text-color="#fff"
    active-text-color="#ffd04b"
    @select="handleSelect"
  >
    <el-menu-item index="7" disabled 
    style="opacity: 0.8;background-color: coral;cursor: default;">甄假账</el-menu-item>
    <el-menu-item index="8" disabled></el-menu-item>
    <el-menu-item index="1">首页</el-menu-item>

    <el-sub-menu index="2">
      <template #title>学习</template>
      <el-menu-item index="2-1">小白学习讨论区</el-menu-item>
      <el-menu-item index="2-2">法律法规指导区</el-menu-item>
      <el-menu-item index="2-3">疑难杂症答疑区</el-menu-item>
      <el-menu-item index="2-4">个性化学习区</el-menu-item>
    </el-sub-menu>
    <el-menu-item index="3">财税服务</el-menu-item>
    <el-sub-menu index="4">
      <template #title>财企汇聚</template>
      <el-menu-item index="4-1">我要招聘</el-menu-item>
      <el-menu-item index="4-2">我要就职</el-menu-item>
    </el-sub-menu>
    <el-menu-item index="5">举报</el-menu-item>
    <el-menu-item index="8" disabled></el-menu-item>
    <el-menu-item index="10" disabled></el-menu-item>
    <el-menu-item index="11" disabled></el-menu-item>
    <el-menu-item index="12" disabled></el-menu-item>
    <el-menu-item index="13" disabled></el-menu-item>
    <el-menu-item index="14" disabled></el-menu-item>
    <el-menu-item index="15" disabled></el-menu-item>
    <el-menu-item index="16" disabled></el-menu-item>
    <el-menu-item index="17" disabled></el-menu-item>
    <el-menu-item index="18" disabled></el-menu-item>

    <el-menu-item index="6">
      <span>个人中心</span>
      <el-icon><User /></el-icon>
    </el-menu-item>
    <el-menu-item index="9" disabled></el-menu-item>
  </el-menu>
  <!-- 搜索框 -->
  <div class="search">
    <el-input v-model="input" 
    placeholder="假账如何甄别" clearable
    style="width: 80%;
    position: absolute;left: 20px;
    top: 10px;
    " @blur="isShow=false" @focus="isShow=true"/>
    <span class="sousuo">搜索</span>
    <el-icon class="sousuotubiao"><Search /></el-icon>
    <div class="tips-app" v-if="isShow">
      <div>如何提高假账检举成功率</div>
      <div>如何提高财会岗位面试竞争力</div>
      <div>如何运用财税新政策进行合理税务规划</div>
      <div>如何提高假账甄别能力</div>
      <div>如何提高实操能力</div>
      <div>重大著名财务造假案例分析</div>
      <div>如何进行合理避税节省企业开支</div>

    </div>
  </div>
  <!-- 词条 -->
  <div class="citiao">
    <span style="font-style: italic;margin-right: 8px;">热门搜索:</span>
    <el-tag class="ml-2" type="info">甄假学习</el-tag>
    <el-tag class="ml-2" type="info">智能税务</el-tag>
    <el-tag class="ml-2" type="info">金税四期</el-tag>
    <el-tag class="ml-2" type="info">财务分析</el-tag>
    <el-tag class="ml-2" type="info">就业经验</el-tag>
    <el-tag class="ml-2" type="info">财务打假</el-tag>
    <el-tag class="ml-2" type="info">财务软件</el-tag>
  </div>
  <component :is="comName" @order="change" @service="change" @report="change"></component>
  </div>
</template>
<script>
import Home from './components/Home/Home.vue' 
import Study1 from './components/Study/Study1.vue' 
import Study2 from './components/Study/Study2.vue' 
import Study3 from './components/Study/Study3.vue' 
import Study4 from './components/Study/Study4.vue' 
import Service from './components/Service/Service.vue'
import Order from './components/Service/Order.vue'
import Enterprises from './components/Talents-enterprises/Enterprises.vue'
import Talents from './components/Talents-enterprises/Talents.vue'
import Report from './components/Report/Report.vue'
import Exposure from './components/Report/Exposure.vue'
import WantReport from './components/Report/WantReport.vue'
import WillReport from './components/Report/WillReport.vue'
import Login from './components/Person/Login.vue'
import Register from './components/Person/Register.vue'
import Person from './components/Person/Person.vue'

export default {
  computed: {
    isperson () {
      if (myCom[5] == 'Person') return true
      else return false
    }
  },
  name:'MyApp',
  components: {
    Home, Study1, Study2, Study3, Study4, Service,Login,Register,Person,
    Order, Enterprises, Talents, Report, Exposure, WantReport,WillReport
  },
  data() {
    return {
      isShow:false,
      comName:"Home",
      myCom:['Home',['Study1','Study2','Study3','Study4'],'Service',['Enterprises','Talents'],'Report','Login']
    }
  },
  methods:{
  handleSelect (key, keyPath)  {
    console.log(key, keyPath)
    if(key==1||key==3||key==5||key==6){
      this.comName = this.myCom[key-1]
    }
    else{
      this.comName = this.myCom[key[0]-1][key[2]-1]
    }
  },
  change(name){
    this.comName = name
    if(name=='Person')this.myCom[5]='Person'
  }
}
}
</script>

<script setup> 

import { ref } from 'vue'
import {
    User,
    Setting,
    Search
} from '@element-plus/icons-vue'
const input = ref('')
const activeIndex = ref('1')
const activeIndex2 = ref('1')


</script> 
<style lang="less">
.tips-app{
  position: absolute;
  background-color: #eae43c;width: 583px;
  height: 200px;top: 41px;z-index: 99;left: 20px;
  >div{
    text-align: left;
    padding: 4px 10px;
    cursor: pointer;
  }
}
.sousuotubiao{
  position: absolute;
  top: 15px;right: 45px;
}
</style>
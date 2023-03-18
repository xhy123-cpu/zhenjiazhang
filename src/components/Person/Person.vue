<template>
  <main>
    <div class="show-bar-person">
        <img src="../../../public/person-img/6.png" id="man">
        <div id="info">
            <div>昵称：admin</div>
            <div>地区：合肥</div>
        </div>
        <div id="huifu">
            <img src="../../../public/person-img/3.png" class="left-person-img">
            <div class="miaoshu-person">回复<br />18</div>
        </div>
        <div id="dianzan">
            <img src="../../../public/person-img/4.png" class="left-person-img">
            <div class="miaoshu-person">获赞数量<br />100</div>
        </div>
        <div id="xuexishichang">
            <img src="../../../public/person-img/1.png" class="left-person-img">
            <div class="miaoshu-person">学习时长<br />58小时</div>
        </div>
        <div id="xuexijifen">
            <img src="../../../public/person-img/2.png" class="left-person-img">
            <div class="miaoshu-person">学习积分<br />99999</div>
        </div>
    </div>
    <div class="main-show-person">
        <div class="main-title">
            收藏课程&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            错题库&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            举报进度&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            聘用消息&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            <div id="jifenshangcheng">
                <img src="../../../public/person-img/5.png" class="biaozhi">
                <div>积分<br />商城</div>
            </div>
            <div id="lishijilu">
                <img src="../../../public/person-img/8.png" class="biaozhi" style="height: 80px;width: 100px;">
                <div>历史<br />记录</div>
            </div>
            <div id="a1"></div>
            <div id="a2"></div>
        </div>
    </div>

  </main>
</template>

<script>
export default {

}
</script>

<style lang="less">
.show-bar-person{
    border-bottom: 10px solid #7ca8ca;
    height: 300px;
    position: relative;
    background-color: #99b6cf;
    #man{
    height: 200px;
    position: absolute;
    top: 50px;
    left: 130px;
    }
    #info{
    position: absolute;
    height: 200px;
    top: 50px;
    width: 270px;
    left: 322px;
    >div{
        height: 100px;
        line-height: 100px;
        font-size: 40px;
    }}

}
#huifu{
    width: 200px;
    height: 100px;
    position: absolute;
    right: 130px;
    top: 50px;
    border-bottom:3px solid #000;
}
#dianzan{
    width: 200px;
    height: 100px;
    position: absolute;
    right: 330px;
    top: 50px;
    border-right:3px solid #000;
    border-bottom:3px solid #000;
}
#xuexishichang{
    width: 200px;
    height: 100px;
    position: absolute;
    right: 330px;
    top: 152px;
    border-right:3px solid #000;
}
#xuexijifen{
    width: 200px;
    height: 100px;
    position: absolute;
    right: 130px;
    top: 152px;
}
.left-person-img{
    height: 80px;
    position: absolute;
    left: 10px;
    top: 10px;
}
.miaoshu-person{
    line-height: 40px;
    font-size: larger;
    height: 80px;
    width: 90px;
    position: absolute;
    right: 30px;
    top: 10px;
}
.main-show-person{
    height: 430px;
    background-color: #fff;
    margin-left: 150px;
    margin-right: 400px;
    margin-top: 20px;
    border-radius: 30px;
    padding: 1px;
    position: relative;
}
.main-title{
    text-align: left;
    margin: 20px 10px;
    padding-left: 20px;
    padding-bottom: 10px;
    border-bottom: 1px solid #000;
    cursor: pointer;
    
}
#jifenshangcheng,#lishijilu,#a1,#a2{
    position: absolute;
    width: 200px;
    height: 100px;
    background-color: #38d5b8;
    right: -240px;
    border-radius: 10px;
    >div{
        position: absolute;
        width: 80px;
        height: 100px;
        font-size: 30px;
        left: 120px;
        top: 10px;
    }

}
#jifenshangcheng{
    top: 0px;
}
#lishijilu{
    top: 110px;
}
#a1{
    top: 220px;
}
#a2{
    top: 330px;
}
.biaozhi{
    width: 100px;
    position: absolute;
    left: 10px;
    top: 10px;
}
</style>
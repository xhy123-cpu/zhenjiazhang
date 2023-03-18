<template>
  <div class="taolun-child">
    <div @click="read(0,$event)">
        <div>入职工作开展</div>
        <ul class="suhongling">
            <li>第一天上班、如何办理工作交接？</li>
            <li>财务负责人可以变更成"我"吗？</li>
            <li>财务部门工作基本流程是什么？</li>
            <li>如何确定会计主体？</li>
            <li>第一次做账，报税，如何快速上手？</li>
            <li>公司使用的财务制度是什么？</li>
            <li>如何知道公司是小规模纳税人还是一般纳税人？</li>
            <li>如何知道公司应该申报哪些税？</li>
            <li>工资、社保、公积金是财务工作还是行政工作？</li>

        </ul>
    </div>
    <div @click="read(1,$event)">
        <div>常见发票问题</div>
        <ul class="suhongling">
            <li>公司收到很多种类不同的发票，如何辨别哪些可以正常入账？</li>
            <li>如何辨别发票真伪？</li>
            <li>公司名下没有车，老板拿过来的加油费、停车、过路费可以做账吗？</li>
            <li>收到只有对方企业名称的发票是否可以使用？</li>
            <li>收到一张发票，上面税额是***，是怎么回事？</li>
            <li>取得发票上盖了两个发票章，一个清楚，一个模糊，能接收吗？</li>
            <li>公司锁坏了，对方开锁人只能提供一张收据，可以做账使用吗？</li>
            <li>公司支付的电费，物业公司只给开具一张收据，没有发票该怎么办？</li>
            <li>收到一张几个月前的发票，还能入账吗？</li>
            <li>收到一张跨年发票应该怎么处理？</li>
            <li>我们为对方开具的发票记账联丢失了，怎么处理？</li>
            <li>取得增值税专用发票，什么时候认证都可以吗？</li>
            <li>取得所有专票上的进项税额都可以认证抵扣吗？</li>
            <li>开票时不知道税收编码应该怎么办，能随便选吗？</li>
            <li>我公司为一般纳税人，可以自己开专票，我们对外的业务都能开专票吗？</li>
            <li>什么情况下发票的备注栏必须要注明？</li>
            <li>发票开错了怎么处理？</li>
            <li>客户让我们开票时金额多开点，他们多抵扣一些成本，可以这样操作吗？</li>
            <li>老板买了一些发票说让做账，想少交点税，应该怎么办？</li>
        </ul>
    </div>
    <div @click="read(2,$event)">
        <div>账务核算问题</div>
        <ul class="suhongling">
            <li>预付下季度房租如何做账？</li>
            <li>预付下季度物业费如何做账？</li>
            <li>预付下年网费如何做账？</li>
            <li>公司发生装修费如何做账？</li>
            <li>支付宝、微信收款如何记账？</li>
            <li>员工出差借款计入什么科目？</li>
            <li>公司向老板或员工借款计入什么科目？</li>
            <li>哪些税费计入税金及附加？</li>
            <li>印花税需要计提吗？</li>
            <li>交社保怎么有的公司用"其他应收款"，有的用"其他应付款"?</li>
            <li>工资的提、发放如何做账？</li>
            <li>公司购买财务软件计入哪个科目？</li>
            <li>应收账款、应付账款怎么区分？</li>
            <li>实务中应收账款需要计提坏账准备吗？</li>
            <li>库存现金盘盈、盘亏怎么处理？</li>
            <li>存货盘盈、盘亏怎么处理？</li>
            <li>固定资产盘盈、盘亏怎么处理？</li>
            <li>无形资产盘盈、盘亏怎么处理？</li>
            <li>餐费发票如何入账？</li>
            <li>银行账户结息计入哪个科目？</li>
        </ul>
    </div>
    <div @click="read(3,$event)">
        <div>涉税实务问题</div>
        <ul class="suhongling">
            <li>税率和征收率的区分？</li>
            <li>如何辨别零税率、免税、不征税？</li>
            <li>什么是含税销售额，什么是不含税销售额？</li>
            <li>混合销售与兼营如何区分？</li>
            <li>小微企业是小型微利企业吗？</li>
            <li>预缴时候多缴的企业所得税，可以在汇算清缴时进行退税吗？</li>
            <li>企业疫情期间发生的亏损能延长8年扣除吗？</li>
            <li>年终奖并入综合所得一起计税，还是单独计税更划算呢？</li>
            <li>享受首套住房贷款利率，但是本月还未开始还贷，首次还贷时间如何填写？</li>
            <li>婚前享受的住房租金扣除，婚后还能继续享受吗？</li>
            <li>第二套房贷利息可以享受住房贷款利息扣除政策吗？</li>
            <li>住房贷款利息和住房租金扣除可以同时享受吗？</li>
            <li>非独生子女赡养老人个税扣除项目可由一人全额扣除吗？</li>
            <li>赡养一位老人和赡养两位老人个税扣除标准一样吗？</li>
            <li>2022年取得初级证书如何抵扣个税？</li>
            <li>专升本学历提升教育如何抵扣个税？</li>
            <li>2022年既取得会计初级证书又进行了专升本学历教育，可以同时抵扣个税吗？</li>
            <li>双胞胎赡养父母是否可以按照独生子女的标准享受个税扣除？</li>
            <li>父母均要满60岁还是只要一位满60岁即可享受扣除？</li>
            <li>合租住房可以分别享受个税扣除政策吗？.</li>
            <li>员工领取原提存的住房公积金需要并入综合所得进行年度汇算吗？</li>
            <li>员工宿舍可以扣除个税房租支出吗？</li>
            <li>员工被辞退取得的一次性补偿收入要并入综合所得计税吗？</li>
            <li>担任公司董事、监事取得的收入是否属于工资薪金？</li>
        </ul>
    </div>
    <div @click="read(4,$event)">
        <div>我的讨论</div>
        <ul class="suhongling">
            <li v-for="item in myDiscuss" :key="item">{{ item }}</li>
        </ul>
    </div>
  </div>
</template>

<script>
export default {
    props:['myDiscuss'],
    methods:{
        read:function(id,e){
            if(document.querySelectorAll('.taolun-child>div')[id].className==='active')
                document.querySelectorAll('.taolun-child>div')[id].className=''
            else
                document.querySelectorAll('.taolun-child>div')[id].className='active'
        }
    }
}
</script>

<style lang="less">
.taolun-child{
    height: 450px;
    overflow-y: scroll;
    >div{
        transition: 0.5s linear;
        overflow: hidden;;
        height: 70px;
        border-bottom: 1px dashed #000;
        border-right: 1px solid #000;
        border-left: 1px solid #000;
        >div{
            height: 70px;
            line-height: 70px;
            font-size: 40px;
            font-weight: bolder;
        }
    }
    .active{
        height: 600px;
        overflow-y: hidden;
    }

}
</style>
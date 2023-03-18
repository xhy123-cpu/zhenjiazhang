<template>
    <div class="taolun-child-2">
      <div @click="read(0,$event)">
          <div>问：通讯补贴需要交纳个税吗？还是可以用通讯发票来报销？</div>
          <ul  class="suhongling"><li>向员工发放通讯费 <br />(1）不需要扣缴个人所得税的情形：<br />手机由公司购买，员工使用手机产生的通讯费由公司承担，发票开给公司，不需扣缴个人所得税；员工个人手机用于公司经营业务，凭发票报销通讯费，财务制度约定标准内不需扣缴个人所得税，超标准部分并入工资薪金所得，扣缴个人所得税。(2）需要扣缴个人所得税的情形：<br />货币发放通讯补贴，应并入工资薪金所得，扣缴个人所得税。</li></ul>
      </div>
      <div @click="read(1,$event)">
          <div>问：个人的社保由公司承担如何入账呢？，做营业外支出可以吗？到时候所得税汇算的时候要调增吗？</div>
          <ul  class="suhongling">
            <li>社保个人部分理应个人承担，现在公司承担了，会计上做账可以进管理费用﹣福利费，但是税法上不认，汇算清缴的时候需要拿出来调增。</li>
          </ul>
      </div>
      <div @click="read(2,$event)">
          <div>问：请问工会经费是每年几月申请退呢？是退100％还是40％还是60％呢？</div>
          <ul  class="suhongling">
            <li>根据工会经费管理规定，企业按工资总额2％计提的工会经费，40％上交总工会，60％直接留企业工会使用。上交总工会的部分，总工会会视企业工会开展工作的情况酌情返还一部分。总工会返还部分和直接留企业工会的60％部分，都归企业工会支配、使用！</li>
            <li>地税代收的工会经费，60％返还基层工会，40％在县以上地方工会、省级产业、厅（局）、集团、公司工会等各层级工会之间进行分配。主要用于上级工会组织开展职工教育、帮扶以及维权等职工活动。</li>
            <li>在总工会网站工会经费收缴管理系统中经过注册程序，填写了基层工会的账户信息并经审核通过，上缴经费的60％将回拨到所填写的工会开户账号中。</li>
            <li>工会经费实行每月返还。地级以上市总工会在收到工会经费后的次月15个工日内，将基层工会应分成部分的工会经费回拨缴费单位工会账户。</li>
          </ul>
      </div>
      <div @click="read(3,$event)">
          <div>问：请问可以以公司名义买商铺吗？怎么抵扣进项呢？</div>
          <ul  class="suhongling">
            <li>可以。根据2019年39号公告的规定：不动产一次性抵扣的政策，主要包括两方面内容：一是，今年4月1日后购入的不动产，纳税人可在购进当期，一次性予以抵扣。二是，今年4月1日前购入的不动产，还没有抵扣的进项税额的40％部分，从2019年4月所属期开始，允许全部从销项税额中抵扣。</li>
          </ul>
      </div>
      <div @click="read(4,$event)">
          <div>问：支付离职研发人员的一次性补偿金能否加计扣除呢？</div>
          <ul  class="suhongling">
            <li>《国家税务总局关于研发费用税前加计扣除归集范围有关问题的公告》（国家税务总局公告2017年第40号）第一条规定，、人员人工费用指直接从事研发活动人员的工资薪金、基本养老保险费、基本医疗保险费、失业保险费、工伤保险费、生育保险费和住房公积金，以及外聘研发人员的劳务费用。依据上述规定，企业按规定标准对研发人员实际支付的离职补偿金，允许税前扣除扣除。但不属于工资薪金，不予加计扣除。</li>    
          </ul>
      </div>
      <div @click="read(5,$event)">
          <div>问：请问研发支出最终的成果是只能转成无形资产还是也可以是固定资产喃？研发费用形成固定资产如何核算？</div>
          <ul  class="suhongling">
            <li>研发支出要么费用化，要么资本化，资本化最终是进无形资产哈，比如，一个工厂研发部门，研发出来拿到国家科委发的专利证什么的。</li>
          </ul>
      </div>
      <div @click="read(6,$event)">
          <div>我的讨论</div>
          <ul  class="suhongling">
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
              if(document.querySelectorAll('.taolun-child-2>div')[id].className==='active')
                  document.querySelectorAll('.taolun-child-2>div')[id].className=''
              else
                  document.querySelectorAll('.taolun-child-2>div')[id].className='active'
          }
      }
  }
  </script>
  
  <style lang="less">
  .taolun-child-2{
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
              line-height: 35px;
              font-size: 30px;
              font-weight: bolder;
          }
      }
      .active{
          height: 1000px;
          overflow-y: hidden;
      }
  
  }
  </style>
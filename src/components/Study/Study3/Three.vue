<template>
    <div class="taolun-child-2">
      <div @click="read(0,$event)">
        <div>基本问题</div>
        <ul  class="suhongling">
            <li>凭证处理<br />1、摘要栏两种快速复制摘要的功能，在下一行中按“..”可复制上一条摘要，按“//”可复制第一条摘要。同时，系统还设计了摘要库，在录入凭证过程中，当光标定位于摘要栏时，按F7或单击「获取」按钮，即可调出凭证摘要库。选择所需的摘要即可，在这个窗口中，您还可以新增、删除或引入摘要；<br />2、会计科目栏会计科目获取——F7或用鼠标单击窗口中的「获取」按钮，可调出会计科目代码；<br />3、金额栏已录入的金额转换方向，按“空格”键即可；若要输入负金额，在录入数字后再输入“-”号即可；<br />4、金额借贷自动平衡——“CTR+F7”<br />5、凭证保存——F8</li>
            <li>凭证审核<br />1、成批审核——先在凭证查询中，“凭证查询”→“全部、全部”，选文件菜单中的“成批审核”功能或按“CTR+H”即可；<br />2、成批销章——先在凭证查询中，“凭证查询”→“全部、全部”，选文件菜单中的“成批销章”功能或按“CTR+V”即可；</li>
            <li>凭证过账<br />1、凭证过账→向导<br />2、凭证反过账——“CTR+F11”</li>
            <li>期末结账<br />1、期末结账：期末处理→期末结账→向导<br />2、期末反结账：CTR+F12</li>
            <li>出纳扎账与反扎账<br />1、出纳扎账：出纳→出纳扎账→向导<br />2、出纳反扎账：CTR+F9</li>
            <li>备份（磁盘或硬盘）<br />1、初始化完、月末或年末，用磁盘备份，插入A盘→文件→备份；<br />2、初始化完、月末或年末，用硬盘备份，文件→备份→选择路径（C盘、D盘、E盘）</li>
            <li>账套恢复<br />想用备份的账套数据（即相应的.AIB 文件），先将备份的账套恢复到硬盘中（恢复为AIS账套文件），再打开它。利用此功能可将备份到软盘上的账套资料恢复到硬盘中。<br />具体操作：文件菜单→恢复→恢复账套→选择备份文件点击后打开→恢复为“AIS”账套；。</li>
            <li>工具菜单<br />1、用户管理（用户增加、删除、授权）；<br />2、用户登录密码（用户密码增加、修改、删除）；<br />3、计算器—F11</li>
        </ul>
      </div>
      <div @click="read(1,$event)">
        <div>账务处理流程</div>
        <ul  class="suhongling">
            <li>凭证录入<br />点击“主窗口”中“凭证录入”，弹出一张凭证的窗口，先修改凭证日期，修改凭证字，输入附件张数，鼠标点到摘要拦，输入摘要内容，此时也可以按F7或者凭证菜单栏里的“获取”按纽，弹出常用摘要窗口，此窗口左下方“增加”按纽增加常用摘要类别（如：收入，支出等）类别名称自编，点右边“增加”按纽增加常用摘要内容，如：提取现金、销售某某商品等等。输入完摘要后，回车，光标跳到会计科目栏，点击“获取”或F7弹出会计科目窗口，在此窗口中选择相应会计科目，也可直接输入科目代码，回车，如果选取的科目关联了核算项目，则光标跳入会计科目左下方的空格，再按F7选择相应的核算项目，然后回车输入金额，继续输入第二条分录，此时输入摘要时可使用快截方式“..”（两个英文状态下的小数点）可复制上条摘要内容→会计科目→金额，此时可使用自动计算平衡“CTRL”+“F7”快捷键功能，系统自动计算出对方金额。→点击“保存”按纽，凭证输入完毕，保存后系统会自动弹出一张空白凭证，继续凭证输入工作。模式凭证：制作完一张常用凭证，如每月都必须做的计提折旧、计提福利费、计提工资等凭证后，点击凭证菜单栏“编辑”，点击“保存为模式凭证”→“常用模式凭证”前打勾，“借方”、“贷方”前打勾→“确定”即可。使用时只要在凭证录入界面，点击凭证上的“编辑”菜单→“调入模式凭证”→选择一张需要的模式凭证→“确定”即可，修改相应的凭证附件张数，凭证日期和相关内容等信息。注意！ 手工输入所有的凭证，但“期末调汇”和“结转损益”凭证除外，此两张凭证需要使用系统提供的自动期末调汇和结转损益功能，否则会导致利润表取不到数。</li>
            <li>凭证查询<br />点击主界面“凭证查询”→弹出凭证过滤窗口，内容中选择“会计期间”“=”“当前会计期间”，窗口下面左边和右面都选“全部”→确定以后显示出本期所有的已保存的凭证，可以在此界面中对凭证进行修改，删除操作，也可直接在此界面中增加新的凭证。修改：双击那张需要修改的凭证，直接修改删除：在会计分录序时簿中，选中那张需要删除的凭证，然后点击菜单拦里红色的“×”，该凭证既被删除，如果前面出现“X”标记，则说明该凭证作废，没有被删除，可点击菜单栏“恢复”按纽恢复该凭证，或者再重复刚才操作既可完全删除该凭证。注意：以上修改删除操作必须是在凭证未审核未过帐状态下方可实现，如该凭证已审核并已过帐，则参照快捷方式及日常操作“反过帐”，“反审核”，恢复凭证到未审核状态！</li>
            <li>更换登陆<br />凭证审核凭证输入完成后，更换操作员登陆金碟点击主界面“凭证审核”→弹出凭证过滤窗口，内容中选择“会计期间”“=”“当前会计期间”，窗口下面左边和右面都选“全部”→确定以后显示出本期所有的凭证→点击菜单栏上“批审”将对序时簿中的凭证批量审核，如选种某张凭证，再点击菜单里的“审核”→弹出该凭证的窗口，再点击凭证菜单上的“审核”是对这张凭证进行单独审核。单独取消审核只需再点击一下凭证菜单栏中的“审核”即可。批量取消审核：用前面审核的操作员登陆，进入“凭证审核”显示出本题的会计分录序时簿，（不要点开任何凭证），单击“编辑”菜单→“成批销章”即可。注意，只可销章本人审核的凭证，其他操作员无权取消他人审核的凭证。</li>
            <li>凭证检查<br />检查本期是否还有未过账的凭证，如本题所有凭证均已过账，点击该按纽，将出现“没有需要检查的凭证”否则，说明本期还有未过账的凭证，需要补做未完工作。</li>
            <li>凭证过账<br />凭证审核完成以后，需要进行过账，点击该项，将出现凭证过账向导，按照提示操作。注意：每期至少需要做两次过账，第一次：结转损益前，对手工制作的所有凭证进行审核过账，第二次：点击“结转损益”，根据提示操作将自动生成一张结转损益的凭证，再对它进行审核过账，有外币业务的企业还必须在结转损益之前使用系统提供的“期末调汇”功能制作一张期末调汇凭证，审核以后再做结转损益工作。此项操作可根据需要适时更换操作员。</li>
            <li>查账<br />本期所有的凭证均过账以后，必须先查看报表和帐簿，才可做结账工作。击金碟主界面左边蓝色导航栏上的“报表”→查看资产负债表/利润表/自定义报表→菜单栏内，“重算”将自动计算出本期报表，如发现报表错误，（如资产负债表不平衡）可退出报表进入账务处理界面，打印一张本期“科目余额表”，再进入报表系统进行核对，对相应错误科目进行报表公式验证，发现错误，进入菜单栏“”进行报表公式修改，修改完毕后，必须回车以后修改有效。1、查询明细账<br />主界面左边“账务处理”→点击右边“明细账”→弹出明细账过滤窗口→选定会计期间→币别→明细科目代码（点击输入框右边的黄色按纽，弹出会计科目窗口选择）。如有核算项目，勾选“包括核算项目”并选择项目类别→包括未过账凭证（此项功能可在凭证未过帐状态查看即时明细帐帐目情况）→确定！系统显示出所需查看科目的明细账，如无发生额和余额，此明细科目账簿不显示。其他账簿，表格等均参照此方法进行过滤查看。<br />2、查询多栏式明细账<br />“账务处理”→“多栏式明细账”→“多栏账”标签页→“增加”→“多栏账科目”选择需要设置多栏账的科目如“管理费用”等，如果此科目未设置下级明细科目而是设置的核算项目，则在“核算项目类别”选择下设的核算项目，如“往来单位”等，（如此科目既未下设明细科目也无核算项目，不能设置成多栏账）→在此窗口左下方点击“自动编排”→“确定”弹出保存为“（所选科目）明细账”→“确定”→到“查询条件”标签页选择相应的会计期间等条件信息→“确定”即可显示出所设置的科目的多栏式明细账。注意！如已经设置过多栏账（如管理费用），之后又增加过此科目的下级明细科目（新费用项目）或核算项目，则再次查询多栏式明细时，必须对此科目进行“修改”，重新“自动编排”一次才能把新增加的明细项目增加到多栏式名细账中，否则会缺少一部分数据。<br />3、查询总账<br />总账以及报表均须所有凭证都过账以后才可显示，打印总账时必须勾选上“按科目分页显示”选项。其他各账务处理过程报表，如科目余额表试算平衡表等和各明细账均可以在凭证未过账状态即可查询即时账簿情况。</li>
        </ul>
      </div>
      <div @click="read(2,$event)">
          <div>操作小技巧</div>
          <ul  class="suhongling">
            <li>凭证处理<br />1、摘要栏两种快速复制摘要的功能，在下一行中按“..”可复制上一条摘要，按“//”可复制第一条摘要。同时，系统还设计了摘要库，在录入凭证过程中，当光标定位于摘要栏时，按F7或单击「获取」按钮，即可调出凭证摘要库。选择所需的摘要即可，在这个窗口中，您还可以新增，删除或引入摘要；<br />2、金额栏已录入的金额转换方向，按“空格”键即可；若要输入负金额，在录入数字后再输入“-”号即可；<br />3、会计科目栏会计科目获取——F7或用鼠标单击窗口中的「获取」按钮，可调出会计科目代码；<br />4、金额借贷自动平衡——“CTR+F7”<br />5、凭证保存——F8</li>
            <li>凭证审核<br />1、成批审核——先在凭证查询中，“凭证查询”→“全部，全部”，选文件菜单中的“成批审核”功能或按“CTR+H”即可；<br />2、成批销章——先在凭证查询中，“凭证查询”→“全部，全部”，选文件菜单中的“成批销章”功能或按“CTR+V”即可；</li>
            <li>凭证过账<br />1、凭证过账→向导<br />2、凭证反过账——“CTR+F11”</li>
            <li>期末结账<br />1、期末结账：期末处理→期末结账→向导<br />2、期末反结账：CTR+F12 （慎用）</li>
            <li>出纳扎账与反扎账<br />1、出纳扎账：出纳→出纳扎账→向导<br />2、出纳反扎账：CTR+F9</li>
            <li>备份（磁盘或硬盘）<br /><br />1、初始化完，月末或年末，用磁盘备份，插入A盘→文件→备份；<br />2、初始化完，月末或年末，用硬盘备份，文件→备份→选择路径（C盘，D盘，E盘）</li>
            <li>账套恢复<br />想用备份的账套数据（即相应的.AIB 文件），先将备份的账套恢复到硬盘中（恢复为AIS账套文件），再打开它。利用此功能可将备份到软盘上的账套资料恢复到硬盘中。具体操作：文件菜单→恢复→恢复账套→选择备份文件点击后→恢复为“AIS”帐套。</li>
            <li>工具<br />1、用户管理（用户增加，删除，授权）；<br />2、用户登录密码（用户密码增加，修改，删除）；<br />3、计算器—F11；<br />4、F12回填</li>
          </ul>
      </div>
      <div @click="read(3,$event)">
        <div>答疑</div>
        <ul  class="suhongling">
            <li>在录入凭证时，为何小数点输不进去？<br />答：这是因为您的输入法状态是全角，解决此问题的方法有两个<br />：（1）您在中文输入法状态下，将全角改为半角即可；<br />（2）您把输入法切换成英文状态即可。</li>
            <li>当凭证录入完毕后，在何处查询？<br />答：在凭证查询中查找。</li>
            <li>当发现凭证输入有错时，该如何处理？<br />答：如果这张凭证是在输入过程中，只需将不正确的地方修改成正确的，保存即可，如果这张凭证已经保存了，首先要在凭证查询中，查到这张凭证，然后用鼠标双击此凭证或直接用工具条中的凭证修改，此时金蝶软件会自动调出这张凭证，您就可进行修改，修改完后保存。注：在修改凭证时以何人的名字进入，保存时制单人即为此人。</li>
            <li>若财务上有两个操作员为A、B，A录入10张凭证，由B审核，但B进行审核时却没看见1张凭证，这是为何？<br />答：在金蝶软件中“用户授权”下有权限适用范围分别为：所有用户、本组用户、本人。现假设C有查询凭证的权限，用它来解释上面三个权限的含义：所有用户：即C可查询到所有财务人员录入的凭证。本组用户：即C可查询到本组财务人员录入的凭证本人：即C只可查询到本人录入的凭证。</li>
            <li>凭证审核过后，发现凭证有错，该如何处理？<br />答：要先进行凭证销章，然后才可修改凭证。首先将此凭证在凭证查询处查出，在文件菜单下（标准版7.0是在编辑菜单下）点成批销章，然后再进行修改。</li>
            <li>如何在有账务发生的情况下增加明细科目？<br />答：先在原科目下增加一个过渡科目，系统会将原科目数据转入这个过渡科目。再将该过渡科目的发生额及余额通过自动转账或制作记账凭证结转到其他新增科目。</li>
            <li>查询科目余额表等报表时，如何查看明细账？<br />金蝶财务软件提供了证账表一体化查询功能。科目余额表（双击）——明细分类账（双击）——记账凭证核算项目明细表（双击）——明细分类账（双击）——记账凭证总分类账（双击）——明细分类账（双击）——记账凭证往来对账单（双击）——记账凭证单位对账单（银行对账）（双击）——记账凭证。</li>
            <li>在金蝶软件中是否只要录入凭证，就可看见账簿和报表？<br />答：只要录入凭证，就可看见明细账，但要看总账和报表，则必须过账。</li>
        </ul>
      </div>
      <div @click="read(4,$event)">
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
<template>
  <div class="tos">
    <div class="screen"></div>
    <div class="box">
      <div class="close" @click="submit('cancel')">
        <i class="icon-close"></i>
      </div>
      <div class="frame">
        <header>{{getTitle()}}</header>
        <article v-if="article === 'service'">
          <p class="title">一、协议主体</p>
          <p>服务接受方，即税易贷平台（anji.shuiyidai.com.cn）用户（个人或企业），包含注册用户和非注册用户。注册用户是指通过anji.shuiyidai.com.cn完成全部注册程序后，使用税易贷平台（anji.shuiyidai.com.cn）服务的用户。非注册用户是指未在税易贷平台（anji.shuiyidai.com.cn）上进行全部注册程序,直接登录anji.shuiyidai.com.cn 或通过其他关联网站授权进入anji.shuiyidai.com.cn使用界面，并使用税易贷平台（anji.shuiyidai.com.cn）服务的用户。</p>
          <p>服务提供方，即浙江数秦科技有限公司运营服务的税易贷平台（anji.shuiyidai.com.cn）（以下简称"税易贷"）。</P>
          <p class="title">二、缔约前提示</p>
          <p>1. 请您在使用税易贷（anji.shuiyidai.com.cn）服务前认真阅读、充分理解全部协议内容。特别是其中所涉及的免除及限制税易贷（anji.shuiyidai.com.cn）责任的条款、对用户权利限制的条款等。请您审慎阅读并选择接受或不接受本协议。若您一旦注册或使用税易贷（anji.shuiyidai.com.cn），则视为您已充分理解并完全接受本协议的全部条款，并无条件地、不可撤销地同意接受的服务，受以下全部条款的约束。如有违反本协议条款而导致任何法律后果，您将独立承担所有相应的法律责任。若您不接受以下条款，请您立即停止注册或停止使用税易贷的服务。</p>
          <p>2. 对于您提供的所有资料及数据信息，一经注册视为您无条件地、不可撤销地在账号使用期内授予税易贷全球通用的、免费的使用权利。</p>
          <p>3. 本协议内容包括但不限于协议正文及所有税易贷（anji.shuiyidai.com.cn）已经发布的或将来可能发布的各类规则。所有规则为本协议不可分割的组成部分，与协议正文具有同等法律效力。除另行明确声明外，税易贷提供的任何服务均受本协议约束。</p>
          <p>4. 税易贷有权根据需要适时的修改本协议及/或各类规则，并在税易贷（anji.shuiyidai.com.cn）上公示，如您不同意相关变更，请停止使用税易贷（anji.shuiyidai.com.cn）服务。如您继续使用税易贷（anji.shuiyidai.com.cn）服务，即表示您无条件、不可撤销地理解并接受新修订的协议和规则。如新旧规则或协议之间冲突或矛盾的，除另行明确声明外，以最新修订的协议和规则为准。</p>
          <p>5. 税易贷是遵循国家税收、银行、征信相关法律法规设立，旨在帮助中小微纳税企业解决融资难的问题而设立的官方服务平台。税易贷遵循自愿服务原则、数据保密原则、公众服务原则。自愿服务原则是注册用户根据自身需要自愿选择税易贷的服务。数据保密原则是税务机关依据国家税收征管法保护纳税人数据安全，银行依据银行业保密规定为客户数据进行保密，税易贷依据征信业管理条例为注册用户的数据保密。</p>
          <p>6. 用户须在税易贷以实名制注册并根据税易贷的要求提供用户自身相关信息，包括但不限于公司名称、联系人、联络信息、工商注册信息、税务登记信息、企业财务信息及资金的需求描述和说明等。用户需遵循税易贷所使用的数据采集方式并对自身提供的信息真实性、完整性、准确性承担全部责任。若您填写的信息不完整，将直接影响税易贷对您资信的分析、通过征信获得银行无抵押贷款。用户应结合自身的财务状况、风险承受能力、风险识别能力等谨慎选择适用由税易贷合作银行提供的金融服务产品，并自行承担因此产生的法律后果。</p>
          <p>7. 凡通过税易贷平台（anji.shuiyidai.com.cn），及其链接的其它网站而获得的网上资料及内容，仅供您浏览和参考之用，请您对相关内容自行辨别及判断，税易贷对上述资料及内容不承担任何责任。</p>
          <p>8. 互联网传输可能会受到干扰、中断、延迟、数据错误、病毒、木马、黑客攻击、系统不稳定、第三方服务瑕疵、政府行为、网络服务平台或相关设备的定期或者不定期检修、维护，非微众税银能控制的通讯设施、硬件故障引致的数据及交易的不准确、不及时或者服务中断，税易贷均不承担任何责任。</p>
          <p>9. 税易贷提供服务过程中涉及的所有内容（包括但不限于网页、文字、图片、音频、视频、图表等）的知识产权归税易贷所有，用户在使用本服务中所产生的内容的知识产权归用户或相关权利人所有。除另有特别声明外，税易贷提供本服务时所依托软件的著作权、专利权及其他知识产权均归税易贷所有。上述及其他任何本服务包含的内容的知识产权均受到法律保护，未经税易贷、用户或相关权利人书面许可，任何人不得以任何形式进行使用或创造相关衍生作品。</p>
          <p class="title">三、 用户的承诺和保证</p>
          <p>1. 在您进行用户的注册程序时，您已是中国籍年满18周岁且具有完全民事行为能力的自然人或已经在工商行政管理局登记注册并有效存续的企业法人。若您不具备前述主体资格，则您及您的监护人应承担因此而导致的一切后果，且税易贷 （anji.shuiyidai.com.cn）有权不经通知直接注销您的帐号（登录名）。</p>
          <p>2. 在您签署本协议，申请税易贷上唯一的用户名，完成注册程序后，请妥善保存税易贷的账号、密码等，用户应对帐号和密码的安全负责，如发现帐号存在异常，请及时与税易贷联系。任何通过您的用户名和密码实施的行为将视为您个人或您的企业的行为，无论是您自己操作还是其他人操作，都由您或您的企业承担全部责任，税易贷不承担任何责任。在未征得税易贷同意的前提下，您不得以任何方式转让、赠与用户名和密码。</p>
          <p>3. 在接受税易贷服务的过程中，用户无条件、不可撤销地承诺不从事下列行为：</p>
          <p>（1） 发表、传送、传播、储存危害国家安全统一、破坏社会稳定、违反公序良俗、侮辱、诽谤、淫秽、暴力以及任何违反国家法律法规的内容；</p>
          <p>（2） 发表、传送、传播、储存侵害他人知识产权、商业秘密等合法权益的内容；</p>
          <p>（3） 制造虚假身份、隐瞒真相、发布虚假信息等误导、欺骗他人，或违背 公布之规则进行虚假交易；</p>
          <p>（4） 进行危害计算机网络安全的行为。</p>
          <p>4. 在税易贷使用服务过程中，用户无条件、不可撤销地承诺遵守以下约定：</p>
          <p>（1） 在使用税易贷过程中实施的所有行为均遵守国家法律、法规及税易贷的各项规则，不违背社会公共利益或公共道德，不损害他人的合法权益。</p>
          <p>（2） 不发布国家禁止发布的信息，不发布其它涉嫌违法或违反本协议及各类规则的信息等。</p>
          <p>（3） 不对税易贷上的任何数据作商业性利用，包括但不限于在未经税易贷事先书面同意的情况下，以复制、传播等任何方式使用税易贷上展示的资料。</p>
          <p>5. 用户无条件、不可撤销地同意并授权：</p>
          <p>（1） 如违反上述承诺时，税易贷有权依据本协议的约定，做出相应处理或终止向您提供服务，且无须征得您的同意或提前通知您。</p>
          <p>（2） 当您的行为涉嫌违反法律法规或违反本协议和/或规则的，税易贷有权采取相应措施，包括但不限于直接屏蔽、删除侵权信息，或直接停止提供服务。如您行为使税易贷遭受任何损失的（包括但不限于受到第三方的索赔、受到行政管理部门的处罚等），您还应当赔偿或补偿税易贷遭受的全部损失及（或）发生的全部费用，包括但不限于诉讼费、律师费、保全费等。</p>
          <p>6. 用户自愿接收国家税务局、银行和税易贷联合提供的持续短信通知服务（短信通知的内容包括但不限于用户的预授信额度总额及余额）。如对用户的日常经营造成影响的，用户可自行通过短信方式取消订阅。用户无条件、不可撤销地承诺不得因此向国家税务局、银行和税易贷投诉或主张任何补偿。</p>
          <p class="title">四、 其他</p>
          <p>1. 本协议之效力、解释、变更、执行与争议解决均适用中华人民共和国法律（香港特别行政区、澳门特别行政区、台湾地区除外），如无相关法律规定，可参照商业惯例和（或）行业习惯。</p>
          <p>2. 因本协议产生的争议，应当协商解决，协商不成可向浙江数秦科技有限公司所在地有管辖权的人民法院起诉。</p>
          <p>3. 税易贷保留对本协议及所有规则的最终解释权。</p>
        </article>
        <article v-if="article === 'business'">
          <p>尊敬的客户：为了维护贵公司的合法权益，请在签署本企业授权协议书（以下简称“本协议书”）前，仔细阅读本协议书全部内容，以知悉贵公司在数据服务中的权利、义务。</p>
          <br>
          <p>一、本公司承诺并确认在签署本协议书前，本公司是依据中国法律注册成立并有效存续的、住所位于中国境内（包括港澳台）的中国企业法人、事业单位及其他经济组织，具有独立承担法律责任的完全民事行为能力。</p>
          <p>二、本公司同意并不可撤销地授权：贵司及下属税易贷（anji.shuiyidai.com.cn，以下简称“平台”）有权按照国家相关规定代本公司收集在使用平台服务中涉及的公司信息和包括信贷信息在内的信用信息、涉税信息（包含但不限于过去24个月内公司基本信息、财务数据、发票明细、申报信息及因未及时履行合同义务产生的不良信息等），前述公司信息和信贷信息如涉及个人税务数据的，均不属于本协议书授权使用范围。本公司对自身提供的所有信息真实性、完整性、准确性承担全部责任。</p>
          <p>三、在本公司成功获得银行授信后，本公司同意并不可撤销地授权：贵司及下属平台有权按照国家相关规定代本公司收集在使用平台服务中涉及的公司信息和包括信贷信息在内的信用信息、涉税信息（包含但不限于公司基本信息、财务数据、发票明细、申报信息及因未及时履行合同义务产生的不良信息等）。在与贷款方结清剩余应还款项之前，贵司及下属平台有权将授权平台收集的动态变更数据提供给贷款方，直至借贷关系解除或终止。</p>
          <p>四、本公司同意授权：本公司接受贵司及下属平台向本公司提供授信额度计算及通知服务，额度计算结果可通过邮件、短信、微信方式通知本公司。在本公司使用该服务期间，授权贵司及下属平台可按照国家相关规定代本公司收集在使用平台服务中涉及的公司信息和包括信贷信息在内的信用信息、涉税信息（包含但不限于公司基本信息、财务数据、发票明细、申报信息及因未及时履行合同义务产生的不良信息等）。本公司可自行通过邮件、短信、微信方式取消该服务。</p>
          <p>五、本公司同意并不可撤销地授权：贵司及下属平台有权根据国家有关规定，在办理涉及本公司所申请的业务时，在经过本公司对所递交所有材料进行确认并同意后，有权使用、打印、保存本公司的信用信息，并用于下述用途：</p>
          <p>（一）移交有关信贷机构审核本公司贷款、贷记卡（信用卡）、准贷记卡申请；</p>
          <p>（二）移交有关信贷机构审核本公司作为提出贷款申请或特约商户申请的组织或机构的出资方、担保方或实际控制方等；</p>
          <p>（三）配合有关信贷机构对已向本公司担任出资方、担保方或实际控制方的机构或组织发放的贷款、贷记卡（信用卡）、准贷记卡进行贷后风险管理；</p>
          <p>（四）向本公司提供贵司及平台的其他信贷业务，除前述（一）、（二）、（三）项外，本公司可根据实际情况选择所需的具体信贷业务。</p>
          <p>六、如果贵司及下属平台超出本协议书范围进行数据报送和查询使用，则贵司及下属平台应承担与此有关的法律责任。本协议书有效期至本公司有关业务办结之日止。</p>
          <p>七、若本公司在贵司及平台所办理的业务未获批准办理，本协议书及本公司信用报告等资料无须退回本公司。</p>
          <p>八、本公司承诺，在使用平台过程中实施的所有行为均遵守国家法律、法规及平台的各项规则，不违背社会公共利益或公共道德，不损害他人的合法权益，不发布国家禁止发布的信息，不发布其它涉嫌违法或违反本协议书及各类规则的信息等，不对平台上的任何数据作商业性利用，包括但不限于在未经贵司及平台事先书面同意的情况下，以复制、传播等任何方式使用平台上展示的资料。</p>
          <p>九、本公司同意贵司及平台提供服务过程中涉及的所有内容（包括但不限于网页、文字、图片、音频、视频、图表等）的知识产权归贵司及下属平台所有。除另有特别声明外，贵司及下属平台提供相关服务时所依托软件的著作权、专利权及其他知识产权均归贵司及下属平台所有。</p>
          <p>十、本公司同意贵司及下属平台有权根据需要适时的修改授权函及/或各类规则，并在平台上公示。本公司同意，如本公司继续使用平台服务，即表示本公司无条件、不可撤销地理解并接受新修订的授权函和规则。</p>
          <p>十一、本公司无条件、不可撤销地承诺，当本公司的行为涉嫌违反法律法规或违反本协议书和/或规则的，贵司及下属平台有权采取相应措施，包括但不限于直接屏蔽、删除侵权信息，或直接停止提供服务。如本公司的行为使贵司及下属平台遭受任何损失的（包括但不限于受到第三方的索赔、受到行政管理部门的处罚等），本公司还应当赔偿或补偿贵司及下属平台遭受的全部损失及（或）发生的全部费用，包括但不限于诉讼费、律师费、保全费等。</p>
          <p>十二、本公司无条件、不可撤销地承诺，应政府机构要求需提供相关证明文件的原件时，本公司将在收到贵司及下属平台的书面通知后【15】日内立即提供。如因本公司未能协助提供相关文件的原件导致国家税务局拒绝协助贵司及下属平台收集税务数据的，本公司将承担所有相关的责任。</p>
          <p>十三、本公司自愿接收贵司及下属平台，以及与贵司合作的政府机构和金融机构向本公司提供的持续短信通知服务（通知的信息包括但不限于贵司及下属平台预测本公司的订单信息、贷款可用额度、平台服务信息、产品信息等）。如对本公司的日常经营造成影响的，本公司可自行通过短信方式取消订阅。本公司无条件、不可撤销地承诺不会因此向贵司及下属平台、以及与贵司合作的政府机构和金融机构投诉或主张任何补偿。</p>
          <p>十四、本公司授权：在第十二条基础上，若本公司符合与贵司合作的金融产品条件，并获得预授信额度，贵司及下属平台可代本公司向贵司合作的金融机构提交申请，但本公司保留撤销该授权的权利，并可以邮件、电话等形式通知贵司。</p>
          <p>十五、本协议书内容与相关业务的合同条款不一致的，无论相关合同在本协议书之前或之后签署，均应以本协议书的内容为准，但相关合同条款明确约定是针对本协议书内容所做修订的除外。</p>
          <p>十六、本公司了解贵司及平台对有关信息的异议和投诉处理规定，同意贵司及平台自收到本公司异议后对相关信息作出存在异议的标注，并自收到异议请求之日起20日内进行核查和处理，同时将结果书面答复本公司。如贵司及平台侵害本公司的合法权益，本公司有权通过向征信主管部门及其派出机构进行投诉或直接向人民法院起诉的方式进行维权。</p>
          <p>十七、本协议书之解释权归属于浙江数秦科技有限公司及下属税易贷。 （以下无正文）</p>
          <p>（本协议书项下授权、承诺行为完全是由本公司独立、自主、谨慎做出。本公司已仔细阅读上述所有条款，并已特别注意字体加黑的内容。平台已应本公司要求对相关条款予以明确说明。本公司对所有条款的含义及相应的法律后果已全部通晓并充分理解，本公司自愿作出上述授权、承诺和声明。）</p>
        </article>
      </div>
      <div class="button-group">
        <div class="read" @click="readProtocol = !readProtocol">
          <i :class="['circle',{'icon-right':readProtocol}]"></i>
          <p v-if="article === 'service'">同意上述服务协议。</p>
          <p v-if="article === 'business'">同意授权使用方访问本公司的基本信息和税务信息。</p>
        </div>
        <p v-if="article === 'business'">（其中税务信息包括：利润表、资产负债表、现金流量表、增值税申报表、所得税申报表、社会保险费缴费申报表、国税纳税总额、地税缴纳总额，纳税信用级别及涉税犯罪行为记录等。）</p>
        <button :disabled="!readProtocol" class="submit" @click="submit('success')">提交</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TosBox',
  data () {
    return {
      readProtocol: false
    }
  },
  props: {
    article: ''
  },
  created () {
  },
  methods: {
    getTitle () {
      switch (this.article) {
        case 'service': return '税易贷服务协议'
        case 'business': return '税易贷企业授权书'
        default: return ''
      }
    },
    submit (msg) {
      this.$emit('submit', msg)
    }
  }
}
</script>

<style lang='scss' scoped>
@import '../../stylesheets/common/tos-box.scss';
</style>

<template>
  <div class="site">
    <img src="../assets/logo-mi2.png" alt="milogo" />
    <div>
      <div>
        <template v-for="(item, i) in links" :key="i">
          <a href="#">{{ item }}</a>
          <span style="margin: 0 0.3em; font-size: 10px; color: #757575" v-if="i !== links.length - 1">|</span>
        </template>
      </div>
      <div>
        <a href="#">北京互联网法院法律服务工作站</a>
        <span style="margin: 0 0.3em; font-size: 10px; color: #757575">|</span>
        <a href="#">中国消费者协会</a>
        <span style="margin: 0 0.3em; font-size: 10px; color: #757575">|</span>
        <a href="#">北京市消费者协会</a>
      </div>

      <div>
        &copy;
        <a href="javascript:;" target="_blank" title="mi.com">mi.com</a> 京ICP证110507号
        <a href="http://beian.miit.gov.cn/" target="_blank" rel="nofollow">京ICP备10046444号</a>
        <a rel="nofollow" href="http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=11010802020134" target="_blank"
          >京公网安备11010802020134号</a
        >
        <a href="//www.mi.com/culture-license/" target="_blank">京网文[2020]0276-042号</a>
        <br />
        <a href="//www.mi.com/medical/record/" target="_blank">（京）网械平台备字（2018）第00005号</a>
        <a href="//www.mi.com/medical/qualification/" target="_blank">互联网药品信息服务资格证 (京)-非经营性-2014-0090</a>
        <a href="//www.mi.com/business-license/" target="_blank">营业执照</a>
        <a href="//www.mi.com/medical/list/" target="_blank">医疗器械质量公告</a>
        <br />
        <a href="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/e0c7d4cf3b7cd88de10196e30c92e020.png" target="_blank">增值电信业务许可证</a
        >&nbsp;网络食品经营备案 京食药网食备202010048 &nbsp;
        <a href="https://cdn.cnbj1.fds.api.mi-img.com/mi-mall/c6859168166651511897f54fa1047fe3.png" target="_blank">食品经营许可证</a>
        <br />
        违法和不良信息举报电话：171-5104-4404&nbsp;<a href="https://www.mi.com/intellectual" target="_blank">知识产权侵权投诉</a
        >&nbsp;本网站所列数据，除特殊说明，所有数据均出自我司实验室测试
      </div>

      <div class="info-links">
        <a
          rel="nofollow"
          href="//privacy.truste.com/privacy-seal/validation?rid=4fc28a8c-6822-4980-9c4b-9fdc69b94eb8&lang=zh-cn"
          target="_blank"
        >
          <img rel="nofollow" src="//i1.mifile.cn/f/i/17/site/truste.png" alt="TRUSTe Privacy Certification" />
        </a>
        <a rel="nofollow" href="//search.szfw.org/cert/l/CX20120926001783002010" target="_blank">
          <img rel="nofollow" src="//s01.mifile.cn/i/v-logo-2.png" alt="诚信网站" />
        </a>
        <a
          id="_xinchacharenzheng_cert_vip_kexinweb"
          rel="nofollow"
          href="//xyt.xinchacha.com/pcinfo?sn=523009637759455232&certType=6"
          target="_blank"
        >
          <img rel="nofollow" src="//xyt.xinchacha.com/img/icon/icon3.png" alt="可信网站" />
        </a>
        <a rel="nofollow" href="//www.mi.com/service/buy/commitment/" target="_blank">
          <img rel="nofollow" src="//i8.mifile.cn/b2c-mimall-media/ba10428a4f9495ac310fd0b5e0cf8370.png" alt="诚信经营 放心消费" />
        </a>
      </div>
    </div>
  </div>

  <div class="slogan"><img src="../../public/xiaomi/slogan2020.png" alt="slogan2020" /></div>
</template>

<script lang="ts" setup>
const links =
  '小米商城|MIUI|米家|米聊|多看|游戏|政企服务|小米天猫店|小米集团隐私政策|小米公司儿童信息保护规则|小米商城隐私政策|小米商城用户协议|问题反馈|Select Location'.split(
    '|'
  )
</script>

<style lang="less" scoped>
.site {
  padding: 20px 0;
  display: flex;
  font-size: 12px;
  img {
    width: 56px;
    height: 56px;
    margin-right: 10px;
  }
  div {
    color: #757575;
    line-height: 1.4;
    a {
      transition: all 0.2s;
      font-size: 12px;
      text-decoration: none;
      color: #757575;
      &:hover {
        color: #ff6700;
      }
    }
  }

  .info-links {
    margin-top: 10px;
    img {
      width: auto;
      height: 28px;
    }
  }
}

.slogan {
  display: flex;
  justify-content: center;
  padding-bottom: 20px;
}
</style>

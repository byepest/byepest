
<template>
  <div class="universal-footer">
    <div class="info-wrapper">

      <div class="contact mb42">
        <div class="f20 lh28 white light">{{contains.common.connect_us}}</div>
        <hr class="white-separator"/>
        <div class="contact-wrapper mt20">
          <div class="columns left flex-column">
            <div class="flex-row mb20">
              <a class="flex-row" :href="'tel:' + contains.common.phone1">
                <img class="icon" src="../assets/img/resources/icon-phone.svg" alt="icon"/>
                <div class="icon_title">{{contains.common.allHotLine}}:</div>
                <div class="category-title hotline ml10 f32 pink-2 bold italic ml8">{{contains.common.phone}}</div>
              </a>
            </div>
            <!--<div class="flex-row mb20 pointer">-->
              <!--<img class="icon" src="../assets/img/resources/icon-location-g.svg"/>-->
              <!--<div class="icon_title" style="width: 72px;">{{$contains.common.headquartersAddress}}:</div>-->
              <!--<div class="category-title ml10 f14 white ml8 light">{{$contains.common.address}}</div>-->
            <!--</div>-->
            <div class="flex-row">
              <a class="flex-row" href="mailto: byepest@bayer.com" data-fuget="175">
                <img class="icon" src="../assets/img/resources/icon-email.svg" alt="icon"/>
                <div class="category-title ml10 f16 white ml8 light">{{contains.common.www}}</div>
              </a>
            </div>

            <div class="wechat flex-row mt20">
              <img class="icon" src="../assets/img/resources/icon-wechat.svg" alt="icon"/>
              <div class="flex-row">
                <div class="category-title ml10 f12 white ml8 light">{{contains.common.search}}</div>
                <div class="input-mock flex-row ml5">
                  <img class="mr4" width="15" height="15" src="../assets/img/resources/icon-magnifier.svg" alt="icon"/>
                  <div class="f12 white light">{{contains.common.object_name}} |</div>
                </div>
              </div>

            </div>
          </div>
          <div class="columns wpa flex-v-center">
            <img width="107" height="107" src="../assets/img/resources/wx_qrcode.png" alt="拜耳虫虫拜拜，拜耳微信公众号二维码"/>
            <div class="qrcode-subtitle mt15 light">{{contains.common.follow_us}}</div>
          </div>
        </div>
      </div>
    </div>

    <div class="diamond-tail header">
      <div class="diamond" style="transform: skewY(-0.878162deg);"></div>
    </div>
    <div class="copyrights-wrapper">

      <div class="copyrights-container">
        <div class="copyrights-content">
          <nuxt-link class="cell flex-row" :to="{path: '/terms'}">
            <img class="disclosure" src="../assets/img/resources/arrow-r.svg"/>
            <div class="cell-title white">{{contains.home.service_terms}}</div>
          </nuxt-link>
          <nuxt-link class="cell flex-row" :to="{path: '/privacy'}">
            <img class="disclosure" src="../assets/img/resources/arrow-r.svg"/>
            <div class="cell-title white">{{contains.home.privacy_statement}}</div>
          </nuxt-link>
          <a class="cell flex-row" :href="contains.common.official_website">
            <img class="disclosure" src="../assets/img/resources/arrow-r.svg"/>
            <div class="cell-title white">{{contains.home.bayer_official_website}}</div>
          </a>
        </div>

        <hr style="background-color: #281D2A;"/>
        <div class="copyrights f12 white light" style="letter-spacing: 1px;">
          © 2018 拜耳作物科学（中国）有限公司 版权所有.
          <span class="interval-space">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>
          浙ICP备18018293号
          <span class="interval-space">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>
          {{contains.common.beian}}
        </div>
      </div>

    </div>
  </div>
</template>

<script>
  import contains from '@/controller/contains'
  export default {
    name: "footer",
    data () {
      return {
        contains: contains,
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../assets/sass/global";
</style>

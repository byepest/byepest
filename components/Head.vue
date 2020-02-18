<template>
  <div class="head">

    <div class="navigator-bar">
      <div class="slogan-wrapper">
        <img class="slogan" :alt="common.object_name" src="../assets/img/resources/slogan.png" style="height: 30px">
      </div>
      <div class="navigator-wrapper">
        <a href="/" class="logo-wrapper flex-row" data-fuget="143">
          <img src="../assets/img/resources/bayer-logo.svg" class="logo" alt="logo">
          <div class="logo-text">{{ common.object_name }}</div>

        </a>
        <div class="menus-wrapper">
          <div class="menus-container">
            <nuxt-link class="menu flex-row" :to="{path: '/'}" >{{home.index}}
            </nuxt-link>
            <div class="slash"></div>
            <nuxt-link class="menu flex-row" :to="{path: '/about'}" >{{home.about}}
            </nuxt-link>
            <div class="slash"></div>
            <a class="menu flex-row nav-menu-expandable" @click="scrollShow = !scrollShow"
            >
              <div>{{home.service_mes}}</div>
              <img class="dropdown ml5" src="../assets/img/resources/icon-enter.png" alt="icon"/></a>
            <div class="slash"></div>

            <nuxt-link class="menu flex-row" :to="{path: '/faq'}" >{{home.need_know}}
            </nuxt-link>

            <div class="slash"></div>
            <nuxt-link class="menu flex-row" :to="{path: '/pest_wiki'}" >
              {{home.pest_mes}}
            </nuxt-link>
          </div>
        </div>

        <div class="hotline-wrapper flex-row" style="flex-direction: row;">
          <img class="icon" width="11" src="../assets/img/resources/phone-pink.svg" alt="icon">
          <div class="hotline ml10 pink-2 semibold italic f23">{{common.phone}}</div>
        </div>

        <div class="action-wrapper flex-v-center">
          <a :href="'tel:' + common.phone1" data-fuget="580">
            <img class="nav-action phone mr15" src="../assets/img/resources/phone.svg" alt="icon">
          </a>
          <img @click="showMenu = !showMenu;showServiceList = false" class="nav-action menu"
               src="../assets/img/resources/menu.svg">
        </div>
      </div>
    </div>

    </div>
  </div>
</template>

<script>
  import contains from '@/controller/contains'
  import datas from '@/controller/data'

  export default {
    name: "Head",
    data() {
      return {
        common: contains.common,
        contains: contains,
        datas: datas,
        home: contains.home,
        scrollShow: false,
        showServiceList: false,
        showMenu: false
      }
    },
    mounted() {
    },
    destroyed() {
    },
    created() {
      // console.log($('.action-wrapper'))
    },
    methods: {
    }
  }
</script>

<style lang="scss" scoped>
  /*@import "../assets/sass/global";*/
  @import "../assets/sass/common";
  @import "../assets/sass/global";

</style>

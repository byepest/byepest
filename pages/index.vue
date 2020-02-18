<template>
  <div class="container">
    <Head></Head>
    <Footers></Footers>
  </div>
</template>

<script>
// import Logo from '~/components/Logo.vue'
import Head from '@/components/Head'
import Footers from '@/components/Footers'
export default {
  components: {
    Head,
    Footers
  },
  head () {
    return {
      title: '拜耳虫虫拜拜'
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

</style>

<template>
  <div class="home">
    <!--<HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <HeaderNav msg="欢迎来到我的第一个vue"></HeaderNav>
    <HomeContent></HomeContent>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import HeaderNav from '@/components/HeaderNav.vue'
import HomeContent from '@/components/HomeContent.vue'

export default {
  name: 'Home',
  components: {
    HeaderNav,
    HomeContent
  }
}
</script>

<style scoped>
</style>

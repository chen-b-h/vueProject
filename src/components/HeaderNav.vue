<template>
  <div id="headerNav">
    <div>
      公共抽奖
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderNav',
  props: {
    msg: String
  }
}
</script>

<style scoped>
  #headerNav{
    background: #FFFFFF;
    position: fixed;
    top: 0;
    width: 100%;
    height: 3em;
  }
  #headerNav>div{
    text-align: center;
    line-height: 3em;
    color: #000000;
  }
</style>

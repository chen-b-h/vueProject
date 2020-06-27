<template>
  <div id="aboutNav">
    <div>
      我的
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutNav',
  props: {
    msg: String
  }
}
</script>

<style scoped>
  #aboutNav{
    background: #FFFFFF;
    position: fixed;
    top: 0;
    width: 100%;
    height: 3em;
  }
  #aboutNav>div{
    text-align: center;
    line-height: 3em;
    color: #000000;
  }
</style>

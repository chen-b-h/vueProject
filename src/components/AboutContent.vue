<template>
<div id="aboutContent">
  <div class="headPic">
    <div class="img">
      <img src="../../public/my/exm2.png">
    </div>
    <div class="heart">
      心愿
      <img src="../../public/my/go.png">
    </div>
  </div>
  <div class="mine">
    <div class="minePri">
      <div class="num">0</div>
      <div class="word">全部抽奖</div>
    </div>
    <div class="minePri">
      <div class="num">0</div>
      <div class="word">发起抽奖</div>
    </div>
    <div class="minePri">
      <div class="num">0</div>
      <div class="word">抽奖记录</div>
    </div>
  </div>
  <div class="prize">
    <img src="../../public/my/exm2.png"/>
    <div class="prizeWord">
      <div>奖品：MAC魅可口红一支 X1</div>
      <div>
        去试试手气
        <img src="../../public/my/go.png" style="width: 20px; height: 20px"/>
      </div>
    </div>
  </div>
  <ul class="listOne list">
    <li v-for="item in listOne" :key="item.id">
      <div class="leftWord">
        <img :src="item.imgUrl" style="width: 24px; height: 24px">
        {{item.leftText}}
      </div>
      <div class="rightWord">
        {{item.rightText}}
        <img src="../../public/image/go.png" style="width: 16px; height: 16px">
      </div>
    </li>
  </ul>
  <ul class="listTwo list">
    <li v-for="item in listTwo" :key="item.id">
      <div class="leftWord">
        <img :src="item.imgUrl" style="width: 24px; height: 24px">
        {{item.leftText}}
      </div>
      <div class="rightWord">
        {{item.rightText}}
        <img src="../../public/image/go.png" style="width: 16px; height: 16px">
      </div>
    </li>
  </ul>
  <ul class="listThree list">
    <li v-for="item in listThree" :key="item.id">
      <div class="leftWord">
        <img :src="item.imgUrl" style="width: 24px; height: 24px">
        {{item.leftText}}
      </div>
      <div class="rightWord">
        {{item.rightText}}
        <img src="../../public/image/go.png" style="width: 16px; height: 16px">
      </div>
    </li>
  </ul>
  <div class="lastText">
    <div>—无码科技产品—</div>
    <div>抽奖超过5000,000,000人次</div>
  </div>
</div>
</template>

<script>
export default {
  name: 'AboutContent',
  props: {
    listOne: {
      type: Array,
      default: () => [
        {
          id: '1',
          imgUrl: require('../../public/my/yue.png'),
          leftText: '余额',
          rightText: ''
        },
        {
          id: '2',
          imgUrl: require('../../public/my/store.png'),
          leftText: '官方商城',
          rightText: 'NoCode Store'
        }
      ]
    },
    listTwo: {
      type: Array,
      default: () => [
        {
          id: '1',
          imgUrl: require('../../public/my/my.png'),
          leftText: '个人主页',
          rightText: ''
        },
        {
          id: '2',
          imgUrl: require('../../public/my/message.png'),
          leftText: '我的消息',
          rightText: ''
        },
        {
          id: '3',
          imgUrl: require('../../public/my/advance.png'),
          leftText: '高级版管理',
          rightText: ''
        },
        {
          id: '4',
          imgUrl: require('../../public/my/daiyanren.png'),
          leftText: '抽奖助手代言人',
          rightText: '限时赚20%'
        }
      ]
    },
    listThree: {
      type: Array,
      default: () => [
        {
          id: '1',
          imgUrl: require('../../public/my/v.png'),
          leftText: '发起人认证',
          rightText: ''
        },
        {
          id: '2',
          imgUrl: require('../../public/my/partner.png'),
          leftText: '推广合作',
          rightText: ''
        },
        {
          id: '3',
          imgUrl: require('../../public/my/mp.png'),
          leftText: '小程序推荐',
          rightText: ''
        },
        {
          id: '4',
          imgUrl: require('../../public/my/more.png'),
          leftText: '更多',
          rightText: ''
        }
      ]
    }
  }
}
</script>

<style scoped>
#aboutContent .headPic{
  margin-top: 4em;
  background: #FAFAFA;
  width: 100%;
  height: 6em;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
#aboutContent .img{
  margin-left: 1.5em;
}
#aboutContent .img img{
  width: 3.5em;
  height: 3.5em;
  border-radius: 50%;
}
#aboutContent .heart{
  margin-right: 1em;
  font-size: 20px;
  font-weight: bolder;
  color: #BB7C39;
}
#aboutContent .heart img{
  width: 20px;
  height: 20px;
}
#aboutContent .mine{
  text-align: center;
  background: #FAFAFA;
  margin-top: 2px;
  width: 100%;
  height: 6em;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
}
#aboutContent .mine .minePri{
  width: 9em;
  border-right: 2px solid #F0F0F0;
}
#aboutContent .mine .minePri:last-child{
  border-right: none;
}
#aboutContent .mine .num {
  font-size: 26px;
  color: #000000;
  font-weight: bold;
}
#aboutContent .mine .word{
  margin-top: 2px;
  color: #808080;
}
#aboutContent .prize{
  display: flex;
  flex-direction: row;
  background: #FFFFFF;
  margin: 10px;
  padding: 10px;
  border: 1px solid #D8D8D8;
  border-radius: 5px;
}
#aboutContent .prizeWord{
  color: #000000;
  font-size: 22px;
  margin-left: 10px;
}
#aboutContent .prize img{
  flex-direction: column;
  width: 100px;
  height: 100px;
}
#aboutContent .prizeWord div:last-child{
  margin-top: 15px;
}
#aboutContent .list{
  background: #FAFAFA;
  list-style: none;
  margin: 0;
  padding: 0;
}
#aboutContent .list li{
  margin-left: 15px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  height: 35px;
  padding: 10px;
  border-bottom: 2px solid #F0F0F0;
}
#aboutContent .leftWord{
  font-size: 24px;
  color: #000000;
}
#aboutContent .rightWord{
  font-size: 20px;
}
#aboutContent .listOne{
  margin-bottom: 10px;
}
#aboutContent .listOne li:last-child{
  border: none;
}
#aboutContent .listTwo{
  margin-bottom: 10px;
}
#aboutContent .listTwo li:last-child{
  border: none;
}
#aboutContent .lastText{
  text-align: center;
  margin-bottom: 50px;
  padding: 50px;
}
#aboutContent .lastText div:first-child{
  font-size: 30px;
  font-weight: bold;
  color: #808080;
}
#aboutContent .lastText div:last-child{
  font-size: 20px;
  color: #808080;
}
</style>

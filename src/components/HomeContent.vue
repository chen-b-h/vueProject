<template>
  <div id="content">
    <div class="ContentNav">
      <div class="navLeft">
        <img class="" src="../../public/image/love.png" style="width:16px;height:16px"/>
        1 心愿
      </div>
      <div class="navRight">
        去签到
        <img class="" src="../../public/image/go.png" style="width:16px;height:16px"/>
      </div>
    </div>
    <div class="navT">
      <div style="font-size:22px;color:#DC3E34;font-weight:bold">
        每日福利
      </div>
      <div class="smallNav">
        <div class="sNavLeft">
          我要上首页
        </div>
        <div class="sNavRight">
          分享
        </div>
      </div>
    </div>
    <ul id="shopItem">
      <li v-for="item in list" :key="item.id">
        <div class="shopping">
          <img :src="item.imgUrl" class="img"/>
          <div class="text">
            <div>{{item.title}}</div>
            <div>{{item.text}}</div>
            <div>{{item.date}}</div>
          </div>
        </div>
      </li>
    </ul>
    <div style="color:#DC3E34;font-size:17px;font-weight:bold;margin:10px">
      自动福利
    </div>
    <ul style="margin:10px" class="teaItem" id="teaItem">
      <li v-for="item in tea" :key="item.id">
        <div class="tea">
          <img :src="item.imgUrl"/>
          <div>
            <div>{{item.text}}</div>
            <div>{{item.date}}</div>
          </div>
        </div>
      </li>
    </ul>
    <div class="contact">
      联系客服
      <img src="../../public/image/go.png"/>
    </div>
    <div class="bImage">
      <img src="../../public/image/exm3.png"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeContent',
  props: {
    list: {
      type: Array,
      default: () => [
        {
          id: '1',
          imgUrl: require('../../public/image/exm1.png'),
          title: 'DC 嘻嘻 赞助',
          text: '一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖',
          date: '6月10号'
        },
        {
          id: '2',
          imgUrl: require('../../public/image/exm1.png'),
          title: 'DC 嘻嘻 赞助',
          text: '一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖',
          date: '6月10号'
        },
        {
          id: '3',
          imgUrl: require('../../public/image/exm1.png'),
          title: 'DC 嘻嘻 赞助',
          text: '一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖',
          date: '6月10号'
        },
        {
          id: '4',
          imgUrl: require('../../public/image/exm1.png'),
          title: 'DC 嘻嘻 赞助',
          text: '一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖一等奖二等奖',
          date: '6月10号'
        }
      ]
    },
    tea: {
      type: Array,
      default: () => [
        {
          id: '1',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '2',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '3',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '4',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '5',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '6',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '7',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '8',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '9',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '10',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        },
        {
          id: '11',
          imgUrl: require('../../public/image/exm2.png'),
          text: '奖品：绿宝石高原绿茶一级铁盒 X10',
          date: '贵茶集团'
        }
      ]
    }
  }
}
</script>

<style scoped>
  #content .ContentNav{
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    margin: 3em 1.5em;
    margin-bottom: 0;
    padding: 1em 0;
    font-size: 16px;
    border-bottom: 2px solid #D8D8D8;
  }
  #content .navT{
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-items: center;
    margin: 0 1.5em;
    padding: 1em 0;
    font-size: 16px;
  }
  #content .smallNav{
    display: flex;
    flex-flow: row nowrap;
    line-height: inherit;
  }
  #content .sNavLeft{
    padding-right: 0.5em;
    border-right: 2px solid #D8D8D8;
  }
  #content .sNavRight{
    padding-left: 0.5em ;
  }
  #shopItem{
    margin: 0;
    padding: 0;
    list-style: none;
  }
  #shopItem .shopping:first-child{
    margin-top: 0
  }
  .shopping{
    display: flex;
    flex-direction: column;
    margin: 12px;
    border: 1px solid #D8D8D8;
    border-radius: 2px;
  }
  .img{
    width: 100%;
    height: 12.5em;
  }
  .text{
    flex-direction: column;
    background: #FFFFFF;
    padding: 15px;
  }
  .text div:first-child{
    color:#DC3E34;
    font-size: 14px;
    font-weight: bold;
    margin-bottom: 5px;
  }
  .text div:last-child{
    color: #E2E0DF;
    font-size: 12px;
    margin-top: 5px;
  }
  #content .teaItem{
    margin: 0;
    padding: 0;
    list-style: none;
  }
  #content .teaItem li:first-child{
    margin-bottom: 10px;
  }
  .tea{
     display: flex;
     flex-direction: row;
     background: #FFFFFF;
     padding: 10px;
     border: 1px solid #D8D8D8;
     border-radius: 5px;
   }
  .tea img{
  flex-direction: column;
    width: 6.25em;
    height: 6.25em;
  }
  .tea div{
    margin-left: 5px;
  }
  .tea div div:first-child{
    font-size: 20px;
  }
  .tea div div:last-child{
    font-size: 16px;
    margin-top: 15px;
  }
  .contact{
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 14px;
    margin: 20px auto;
  }
  .contact img{
    width: 16px;
    height: 16px;
  }
  .bImage{
    margin: 0 10px;
    margin-bottom: 3em;
    padding-bottom: 50px;
  }
  .bImage img{
    width: 100%;
    height: 6.25em;
  }
</style>

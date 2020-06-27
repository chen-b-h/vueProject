<template>
  <div id="app">
    <div id="nav">
      <div id="NavFlex">
        <div class="singleNav">
          <router-link to="/">
            <div>
              <img src="../public/image/index_2.png" style="width: 30px;height: 30px"/>
            </div>
            首页
          </router-link>
        </div>
        <div class="singleNav">
          <router-link to="/Prize">
            <div>
              <img src="../public/image/gift_1.png" style="width: 30px;height: 30px"/>
            </div>
            发起抽奖
          </router-link>
        </div>
        <div class="singleNav">
          <router-link to="/about">
            <div>
              <img src="../public/image/my_1.png" style="width: 30px;height: 30px"/>
            </div>
            我的
          </router-link>
        </div>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  a {
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;

    &.router-link-exact-active {
      color: red;
    }
  }
  position: fixed;
  bottom: 0;
  width: 100%;
  height: 4em;
  background-color: #FFFFFF;
}
#NavFlex{
  //text-align: center;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-content: center;
}
#NavFlex>div{
  font-size: 18px;
}
#NavFlex .singleNav{
  text-align: center;
}
</style>

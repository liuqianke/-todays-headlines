	<template>
  <div id="app">
    <h1>今日头条</h1>
    <i class="toutiao toutiao-shipin"></i>
    <van-button type="primary">主要按钮</van-button>
    <van-button type="info">信息按钮</van-button>
    <van-button type="default">默认按钮</van-button>
    <van-button type="warning">警告按钮</van-button>
    <van-button type="danger">危险按钮</van-button>
    
    <van-cell-group>
      <van-cell title="单元格" value="内容" />
      <van-cell title="单元格" value="内容" label="描述信息" />
    </van-cell-group>
     <router-view />
    <div class="box" style="padding:20px">hello world!!!</div>
  </div>
</template>

<script>
import Vue from 'vue';
import { Button } from 'vant';
import { Cell, CellGroup } from 'vant';

Vue.use(Cell);
Vue.use(CellGroup);
Vue.use(Button);
export default {
  name: 'App'
}
</script>
<style scoped lang="less">
.box{
  width: 200px;
  height: 200px;
  background-color: aqua;
  font-size: 50px;
}
</style>
				
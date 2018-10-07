<template>
  <div>
    <ul class="listview">
      <li>花间一壶酒</li>
      <li>独酌无相亲</li>
      <li>举杯邀明月</li>
      <li>对影成三人</li>
    </ul>
    <div class="title">这是什么鬼</div>
    <div class="items">
      <div class="item">
        <div class="name">哈哈</div>
        <div class="value">孤独</div>
      </div>
      <div class="item">
        <div class="name">给爷笑一个</div>
        <div class="value">没有兑现</div>
      </div>
      <div class="item">
        <div class="name">好吧:</div>
        <div class="value">纯粹</div>
      </div>
      <div class="item">
        <div class="name">没有人告诉他么</div>
        <div class="value">你们好</div>
      </div>
      <div class="item">
        <div class="name">就你能的</div>
        <div class="value">悲伤的感觉</div>
      </div>
      <div class="item">
        <div class="name">有意思</div>
        <div class="value">牛逼</div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        electron: process.versions.electron,
        name: this.$route.name,
        node: process.versions.node,
        path: this.$route.path,
        platform: require('os').platform(),
        vue: require('vue/package.json').version
      }
    }
  }
</script>

<style scoped>
  .title {
    color: #888;
    font-size: 18px;
    font-weight: initial;
    letter-spacing: .25px;
    margin-top: 10px;
  }

  .items { margin-top: 8px; }

  .item {
    display: flex;
    margin-bottom: 6px;
  }

  .item .name {
    color: #6a6a6a;
    margin-right: 6px;
  }

  .item .value {
    color: #35495e;
    font-weight: bold;
  }
  .listview {
    color: red;
    background-color: aqua;
  }

</style>

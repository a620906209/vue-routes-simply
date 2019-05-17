<template>
  <div id="app">
    <h1 id="foot">I am footer</h1>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>

#foot{
  background-color: red;
  box-sizing: border-box;
    /* 設定footer絕對位置在底部 */
  position: absolute;
  bottom: 0;
    /* 展開footer寬度 */
  width: 100%;
}

</style>

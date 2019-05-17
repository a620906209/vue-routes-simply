<template>
    <div class="container">
      <header>
        <slot name="header"></slot>
      </header>
      <main>
        <slot></slot>
      </main>
      <footer>
        <slot name="footer"></slot>
      </footer>
    </div>
</template>


<script>
export default {
  props: ['id']
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

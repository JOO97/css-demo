<template>
  <!-- grid-网格布局-二维 -->
  <div class="wrapper">
    <div style="grid-area: head">head</div>
    <div style="grid-area: nav">nav</div>
    <div style="grid-area: main">main</div>
    <div style="grid-area: footer">footer</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {}
}
</script>

<style scoped lang="scss">
.wrapper {
  display: grid;
  height: 100vh;
  width: 100%;
  grid-template-columns: 100px 1fr;
  grid-template-rows: 60px 1fr 40px;
  grid-gap: 10px 5px;
  grid-template-areas: 'head head' 'nav main' 'nav footer';
  div {
    background: pink;
  }
}
</style>

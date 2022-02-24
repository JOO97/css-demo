<template>
  <!-- holy grail 双飞翼布局-->
  <div class="wrapper">
    <div style="grid-area: head">head</div>
    <div style="grid-area: nav">nav</div>
    <div style="grid-area: main">main</div>
    <div style="grid-area: nav2">nav2</div>
    <div style="grid-area: footer">footer</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {}
  },
  methods: {}
}
</script>

<style scoped lang="scss">
.wrapper {
  height: 100vh;
  display: grid;
  grid-template-rows: 60px 1fr 40px;
  grid-template-columns: 100px 1fr 100px;
  grid-template-areas: 'head head head' 'nav main nav2' 'footer footer footer';
  div {
    background: pink;
  }
}
</style>

<template>
  <div class="container">
    <div class="border-all"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style scoped lang="scss">
.container {
  width: 50px;
  height: 50px;
  position: relative;
}
.border-all {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 200%;
  height: 200%;
  border: 1px solid #000;
  transform: scale(0.5);
  transform-origin: 0 0;
}
</style>

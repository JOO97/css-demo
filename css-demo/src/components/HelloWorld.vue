<template>
  <div class="wrapper">
    <div class="item"></div>
    <div class="item"></div>
    <!-- <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div> -->
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
  margin: 10px;
  height: 100px;
  width: 100px;
  background: #e7e7e7;
  border-radius: 5px;
  display: flex;
  //1
  align-items: center;
  justify-content: center;
  //6
  // flex-wrap: wrap;
  // align-items: center;
}
.item {
  position: relative;
  width: 50%;
  &::after {
    content: '';
    position: absolute;
    width: 20px;
    height: 20px;
    border-radius: 50%;
    background: #000;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>

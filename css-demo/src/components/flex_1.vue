<template>
  <div class="box">
    <div id="box1">box1</div>
    <div id="box2">box2</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {}
}
</script>

<style scoped lang="scss">
.box {
  height: 200px;
  display: flex;
}
#box1 {
  background-color: lightcoral;
  flex-basis: 80%;
}
//flex:1;
//flex: 1 1 auto;
//flex-grow:1;flex-shrink:1;flex-basic:0%;
//默认flex: 0 1 auto;

//flex: 0;
//flex-grow:0;flex-shrink:1;flex-basic:0%;

//flex: 0%;
//flex-grow:1;flex-shrink:1;flex-basic:0%;

//flex: 24px;
//flex-grow:1;flex-shrink:1;flex-basic:24px;

#box2 {
  background-color: lightpink;
  flex-basis: 100px;
}
</style>

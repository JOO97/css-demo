<template>
  <div class="wrapper">
    <!-- 1-3 -->
    <!-- <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div> -->
    <!-- 4 -->
    <!-- <div class="row">
      <div class="item">1</div>
      <div class="item">2</div>
    </div>
    <div class="row">
      <div class="item">3</div>
      <div class="item">4</div>
    </div> -->
    <!-- 5 -->
    <div class="row">
      <div class="item"></div>
      <div class="item"></div>
    </div>
    <div class="row">
      <div class="item"></div>
    </div>
    <div class="row">
      <div class="item"></div>
      <div class="item"></div>
    </div>
    <!-- 6 -->
    <!-- <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
    <div class="item">4</div>
    <div class="item">5</div>
    <div class="item">6</div> -->
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
  //1---------------------------
  // align-items: center;
  // justify-content: center;
  //2-------------------------------------
  // justify-content: space-between;
  // .item {
  //   &:nth-child(2) {
  //     align-self: flex-end;
  //   }
  // }
  //3-------------------------------
  // justify-content: space-around;
  // .item {
  //   &:nth-child(2) {
  //     align-self: center;
  //   }
  // &:nth-child(3) {
  //   align-self: flex-end;
  // }
  // }
  //4----------------------------
  // flex-wrap: wrap;
  // //多轴时，生效
  // align-content: space-between;
  // .row {
  //   display: flex;
  //   justify-content: space-between;
  //   width: 100%;
  // }
  //5--------------------
  justify-content: space-between;
  .row {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    &:nth-child(2) {
      justify-content: center;
    }
  }
  //6---------------------
  // flex-wrap: wrap;
  // align-items: center;
  // flex-direction: column;
  // align-content: space-between;
}
.item {
  position: relative;
  width: 24px;
  height: 24px;
  border-radius: 50%;
  margin: 4px;
  color: white;
  text-align: center;
  background-color: #333;
  box-shadow: inset 0 3px #111, inset 0 -3px #555;
  // &::after {
  //   content: '';
  //   position: absolute;
  //   width: 20px;
  //   height: 20px;
  //   border-radius: 50%;
  //   background: #000;
  //   top: 50%;
  //   left: 50%;
  //   transform: translate(-50%, -50%);
  // }
}
</style>

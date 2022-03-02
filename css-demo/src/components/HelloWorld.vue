<template>
  <div class="wrapper">
    <!-- <div class="row">
      <div style="height: 200px">1</div>
      <div style="clear: both">2</div>
    </div> -->
  </div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style lang="scss">
//居中
// body {
//   //1
//   // display: flex;
//   // justify-content: center;
//   // align-items: center;
//   //2
//   // position: relative;
//   //3
//   position: relative;
//   .wrapper {
//     //2
//     // position: absolute;
//     // left: 50%;
//     // top: 50%;
//     // transform: translate(-50%, -50%);
//     // width: 50px;
//     //3
//     position: absolute;
//     left: 0;
//     right: 0;
//     top: 0;
//     bottom: 0;
//     margin: auto;
//     height: 50px;
//     width: 50px;
//     background: pink;
//   }
// }

//clear
// .wrapper {
//   .row {
//     margin-bottom: 5px;
//     div {
//       background: pink;
//       &:nth-child(n) {
//         float: left;
//       }
//     }
//     &:nth-child(1) {
//       //1
//       // overflow: auto;
//       //2
//       // &::after {
//       //   content: '';
//       //   display: block;
//       //   clear: both;
//       // }
//     }
//   }
// }

//triangle

// .wrapper {
//   width: 0;
//   height: 0;
//   border-style: solid;
//   border-width: 0 50px 50px;
//   border-color: transparent transparent pink transparent;
// }
</style>

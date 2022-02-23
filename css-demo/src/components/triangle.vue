<template>
  <div class="wrapper">
    <div class="c-1"></div>
    <!-- 三角 -->
    <div class="c-2"></div>
    <!-- 镂空三角 -->
    <div class="c-3"></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  
}
</script>

<style scoped>
.c-1 {
  width: 50px;
  height: 50px;
  border-color:pink red skyblue green;
  border-style: solid;
  border-width: 50px 50px 50px;
}
.c-2 {
  width: 0;
  height: 0;
  border-color:transparent transparent skyblue transparent;
  border-style: solid;
  border-width: 0 50px 50px;
}
.c-3 {
   width: 0;
  height: 0;
  border-color:transparent transparent skyblue transparent;
  border-style: solid;
  border-width: 0 50px 50px;
  position: relative;
}
.c-3::after{
  content: '';
  position: absolute;
  width: 0;
  height: 0;
  border-color:transparent transparent #fff transparent;
  border-style: solid;
  border-width: 0 40px 40px;
  left: -40px;
  top: 6px;

}
</style>

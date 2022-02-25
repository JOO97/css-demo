<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100vw;
  height: 100vh;
  .home {
    width: 100%;
    height: 100%;
  }
}
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

html {
  //禁止左右滑动
  // touch-action: none;
  // touch-action: pan-y;
  // width: 100vw;
  // overflow-x: hidden;
}
</style>

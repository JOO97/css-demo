<template>
  <div class="wrapper">joo</div>
</template>

<script>
export default {
  name: 'HelloWorld'
}
</script>

<style lang="scss">
html {
  // 100vw / 375 = x / 100
  // font-size: 4.266667vw; //让1rem = 100px
}
body {
  font-size: 100px;
}
/* max-width：1401 大于时才会应用 */
@media (min-width: 1401px) {
  .wrapper {
    background: #f1f1f1;
  }
}
/* max-width：1400 小于时才会应用 */
@media (max-width: 1400px) {
  .wrapper {
    background: #000;
  }
}

@media (max-width: 1200px) {
  .wrapper {
    background: pink;
  }
}

@media (max-width: 992px) {
  .wrapper {
    background: skyblue;
  }
}

@media (max-width: 768px) {
  .wrapper {
    background: yellowgreen;
  }
}

@media (max-width: 576px) {
  .wrapper {
    background: green;
  }
  body {
    font-size: 50px;
  }
}
</style>

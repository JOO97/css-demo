<template>
  <div class="wrapper">
    <div v-for="item in list" :key="item" :style="{ height: item + 'px' }">
      {{ item }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      list: [
        '70',
        '80',
        '185',
        '62',
        '90',
        '100',
        '75',
        '162',
        '88',
        '97',
        '86',
        '180'
      ]
    }
  },
  methods: {}
}
</script>

<style scoped lang="scss">
.wrapper {
  width: 900px;
  column-count: 5;
  column-gap: 5px;
  div {
    // width: 200px;
    border: 1px solid #ccc;
    text-align: center;
    break-inside: avoid;
    margin-bottom: 5px;
  }
}
</style>

<template>
  <div>cccccccc123123 cccc cccccc sdasd</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {}
}
</script>

<style scoped lang="scss">
div {
  width: 100px;
  border: 1px solid #000;
  // overflow: hidden;
  // text-overflow: ellipsis;
  // white-space: nowrap;

  // overflow: hidden;
  // text-overflow: ellipsis;
  // display: -webkit-box;
  // -webkit-line-clamp: 2;
  // -webkit-box-orient: vertical;
  // word-break: break-all;

  position: relative;
  line-height: 1.5em;
  height: 3em;
  overflow: hidden;
  &::after {
    content: ',,,';
    position: absolute;
    bottom: 0;
    right: 0;
    padding: 0 5px;
    background-color: #fff;
  }
}
</style>

<template>
  <div>
    <div class="wrapper" ref="box" id="box"></div>
    <button @click="move">move</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {
    move() {
      console.log(1)
      // const { box } = this.$refs
      const box = document.getElementById('box')
      console.log(box.offsetLeft)
      let timer = setInterval(() => {
        let speed = 10
        if (box.offsetLeft != 1000) {
          box.style.left = box.offsetLeft + speed + 'px'
        } else {
          clearInterval(timer)
        }
      }, 50)
    }
  }
}
</script>

<style scoped lang="scss">
.wrapper {
  width: 50px;
  height: 50px;
  border: 1px solid #000;
}
</style>

<template>
  <div>
    <div class="js">
      <div class="wrapper" ref="box" id="box"></div>
      <button @click="move">move</button>
    </div>
    <div class="css">
      <div class="wrapper"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {
    move() {
      const box = document.getElementById('box')
      let timer = setInterval(() => {
        let speed = 10
        if (box.offsetLeft != 100) {
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
.js {
  position: relative;
  .wrapper {
    width: 50px;
    height: 50px;
    border: 1px solid #000;
    position: absolute;
    left: 0;
    top: 0;
  }
  button {
    margin-top: 100px;
  }
}
.css {
  position: relative;
  width: 100px;
  height: 400px;

  div {
    border: 1px solid #000;
    width: 50px;
    height: 50px;
    position: absolute;
    left: 0;
    top: 0;
    // animation: move 1s linear 1s;
    transition: transform 2s;
    &:hover {
      transform: translateX(200px) translateY(100px);
    }
    @keyframes move {
      20% {
        left: 20px;
      }
      40% {
        left: 40px;
      }
      60% {
        left: 60px;
      }
      80% {
        left: 80px;
      }
      100% {
        left: 100px;
      }
    }
  }
}
</style>

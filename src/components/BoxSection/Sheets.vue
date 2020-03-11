<template>
  <div class="wrapper" :class="{active: isActive}">
    <div class="sheet">
      <div class="exit" @click="exitSheet">
        <i class="fas fa-times"></i>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    isActive: Boolean
  },
  methods: {
    exitSheet() {
      let changeInActive = this.isActive;
      changeInActive = !changeInActive;
      this.$emit("closeSheet", changeInActive);
    }
  }
};
</script>
<style lang="scss" scoped>
.active {
  height: 100%;
}
.wrapper {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(10px);
  z-index: 2;
  transition: 2s;
  .sheet {
    position: relative;
    top: 55%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #fff;
    max-width: 800px;
    width: 90%;
    height: 70%;
    max-height: 700px;
    border-radius: 30px;
    .exit {
      position: absolute;
      top: 30px;
      right: 30px;
      cursor: pointer;
      i {
        font-size: 30px;
        color: #2d3681;
      }
    }
  }
}
</style>
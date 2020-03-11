<template>
  <div>
    <div class="wrap">
      <div class="container">
        <div class="row">
          <div class="col-10 mx-auto nav">
            <img src="../../assets/LogoMain.png" alt />
          </div>
          <div class="col-1 ham">
            <div class="hamburger" @click="isActive = !isActive">
              <div></div>
              <div></div>
              <div></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Navigation :isActive="isActive" />
  </div>
</template>
<script>
import Navigation from "./Navigation.vue";
export default {
  data() {
    return {
      isActive: false
    };
  },
  components: {
    Navigation
  }
};
</script>
<style lang="scss" scoped>
.wrap {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 4;
  background-color: #fff;
  border-bottom: 2px solid #0b70b8;
}
.container {
  height: 100px;
  max-width: 1100px;
  margin: 0 auto;
  z-index: 5;
}
.row {
  width: 100%;
  display: flex;
  align-items: center;
  div {
    padding: 0;
  }
  .nav {
    img {
      height: 100px;
      margin-top: -7px;
    }
  }
  .ham {
    margin-right: 10px;
    margin-top: 7px;
    .hamburger {
      cursor: pointer;
      div {
        width: 50px;
        height: 6px;
        background-color: #2d3681;
        border-radius: 10px;
        margin-bottom: 6px;
      }
    }
  }
}
</style>
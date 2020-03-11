<template>
  <div>
    <div class="mobile" :class="{unhiden: isActive}">
      <div class="container">
        <div class="row">
          <div class="col-12 col-md-2 mx-auto" v-for="item in menu" :key="item">
            <a href>{{item}}</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      menu: ["Galeria", "Cennik", "Grafik", "O nas", "Kontakt"]
    };
  },
  props: {
    isActive: Boolean
  },
  methods: {
    mobileMenu() {
      this.isActive = !this.isActive;
    }
  }
};
</script>
<style lang="scss" scoped>
.mobile {
  position: fixed;
  top: -400px;
  left: 0;
  width: 100%;
  z-index: 3;
  transition: 0.3s;
  .container {
    margin: 0 auto;
    .row {
      margin: 0;
      padding: 0;
      background-color: #fff;
      border-bottom-left-radius: 30px;
      border-bottom-right-radius: 30px;
      border: solid 2px #0b70b8;
      div {
        list-style: none;
        font-size: 20px;
        width: 120px;
        text-align: center;
        a {
          color: #2d3681;
          display: block;
          line-height: 90px;
        }
        a:hover {
          text-decoration: none;
          font-weight: 700;
        }
      }
    }
  }
}
.unhiden {
  top: 100px;
  transition: 0.3s;
}
</style>
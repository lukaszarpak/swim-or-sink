<template>
  <div class="wrap">
    <div class="container">
      <div class="row">
        <div class="col-10 col-md-6 box mx-auto">
          <div class="description">
            <p>Zobacz zdjęcia z zajęć</p>
            <button>Galeria</button>
          </div>
        </div>
        <div class="col-10 col-md-6 box mx-auto">
          <div class="container">
            <div class="row">
              <div class="col-6 boxIn"></div>
              <div class="col-6 boxIn">
                <div class="description">
                  <p>Grafik zajęć</p>
                  <button>Zobacz</button>
                </div>
              </div>
              <div class="col-6 boxIn">
                <div class="description">
                  <p>Przeczytaj więcej o nas</p>
                  <button>Poznaj nas</button>
                </div>
              </div>
              <div class="col-6 boxIn"></div>
            </div>
          </div>
        </div>
        <div class="col-10 col-md-6 box mx-auto">
          <div class="description">
            <p>
              Zobacz ceny
              klikając poniżej
            </p>
            <button @click="isActive = !isActive">Cennik</button>
          </div>
        </div>
        <div class="col-10 col-md-6 box mx-auto">
          <div class="description">
            <p>Poznaj naszych trenerów</p>
            <button>Trenerzy</button>
          </div>
        </div>
      </div>
    </div>
    <Sheets :isActive="isActive" @closeSheet="update" />
  </div>
</template>
<script>
import Sheets from "./Sheets.vue";
export default {
  data: function() {
    return {
      isActive: false
    };
  },
  methods: {
    update(active) {
      this.isActive = active;
    }
  },
  components: {
    Sheets
  }
};
</script>
<style lang="scss" scoped>
.wrap {
  padding: 150px 0 150px 0;
  background-color: #102c4f;
}

.box {
  height: 400px;
  background-color: #ff0066;
  .description {
    color: #fff;
    width: 100%;
    text-align: center;
    margin-top: 160px;
    height: 100px;
  }
}

.box:first-of-type {
  background-image: url("../../assets/swimmingBoy.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 50% 50%;
}

.box:nth-of-type(4) {
  background-image: url("../../assets/trener1.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 50% 50%;
}

.container {
  .container {
    width: 100%;
    padding: 0;
    margin: 0;
  }
}

.boxIn {
  height: 200px;
  margin: 0;
  padding: 0;
  .description {
    color: #fff;
    width: 100%;
    text-align: center;
    margin-top: 60px;
    height: 100px;
  }
}
.boxIn:first-of-type {
  background-image: url("../../assets/swimmingGirl.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 50% 50%;
}

.boxIn:nth-of-type(4) {
  background-image: url("../../assets/swimmingClasses.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 50% 50%;
}

button {
  color: #fff;
  background: none;
  border: 2px solid #fff;
  border-radius: 30px;
  padding: 10px 20px;
  width: 160px;
  font-weight: 700;
  transition: 0.2s;
}
button:hover {
  background: #fff;
  color: #ff0066;
}
button:focus {
  outline: none;
}
</style>
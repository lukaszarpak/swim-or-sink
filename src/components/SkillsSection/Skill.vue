<template>
  <div class="col-8 col-sm-7 col-lg-3 mx-auto mb-5 sheets">
    <img src="../../assets/photo1.jpg" alt />
    <h3>Początkujący</h3>
    <p>Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor</p>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.sheets {
  border: 5px solid #2fc0df;
  border-radius: 30px;
  color: black;
  background-color: #fff;

  > img {
    width: 90%;
  }
  > h3 {
    color: #102c4f;
  }
}
</style>
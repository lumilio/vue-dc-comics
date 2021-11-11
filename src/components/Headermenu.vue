<template>
  <div class="box-C1">
      <div class="layout-box">
          <div class="centered-box">
                <img src="../assets/img/dc-logo.png" alt="">
                <div>xxx</div>
          </div>
          
      </div>
  </div>
</template>




<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>





<style scoped lang="scss">
@import '../assets/scss/variables.scss';
.box-C1{
    @include layout-block-1;
}
.layout-box{
    @include layout-block-1;
    margin-top: 1rem;
    background-color: white;
}
.centered-box{
    @include layout-block-2;
    justify-content: space-between;
}
.centered-box img{
    width: 100px;
    height: 100px;
}
</style>
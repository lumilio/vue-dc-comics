<template>
    <li>  <a href="#"><img :src="image" alt="">{{label}}</a></li>
</template>



<script>
export default {
  name: 'C3-1',
  components:{},
  props: {
    image: String,
    label: String,

  }
}
</script>



<style scoped lang="scss">
@import '../assets/scss/variables.scss';
.box-C2{
    @include layout-block-1;
}
.layout-box{
    @include layout-block-1;
}
.centered-box{
    @include layout-block-2;
    height: 95px;
    font-size: large;
    color: white;
}
</style>
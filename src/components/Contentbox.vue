<template>
    <div class="box-C1">
        <div class="layout-box">
            <div class="centered-box">
                Contents goes here ...
            </div>
        </div>
    </div>
</template>



<script>
export default {
  name: 'C2',
  components:{},
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
}
.centered-box{
    @include layout-block-2;
    height: 95px;
    font-size: large;
    color: white;
}
</style>
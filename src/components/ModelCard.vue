<template>
    <div class="card-model">
        <img :src="thumb" alt="">
        <p>{{series}}</p>
    </div>
</template>



<script>
export default {
  name: 'C2-1',
  components:{},
  props: {
    thumb: String,
    series: String,
  }
}
</script>



<style scoped lang="scss">
</style>
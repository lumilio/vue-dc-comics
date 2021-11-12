<template>
    <div class="card-model">
        <img :src="thumb" alt="">
        <p>{{series.toUpperCase()}}</p>
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
.card-model {
    padding: 0.6rem;
}
.card-model img{
    width: 170px;
    height: 170px;
    object-fit: cover;
    object-position: center top;
}
.card-model p{
    width: 120px;
    margin-top: 8px;
    margin-bottom: 16px;
}
</style>
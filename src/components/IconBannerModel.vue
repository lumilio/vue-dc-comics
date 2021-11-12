<template>
    <li>  <a href="#"><img :src="require(`../assets/img/${image}`)" alt="">{{label}}</a></li>
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
li {
    display: inline-block;
    font-size: 13px;
}
a {
    display: flex;
    color: white;
    align-items: center;
    text-decoration: none;
}
li > a > img{
    height: 40px ;
    padding: 10px;
}
</style>
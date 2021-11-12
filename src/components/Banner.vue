<template>
    <div class="box-C3">
        <div class="layout-box">
            <div class="centered-box">
                <ul id='banner-list'>
                    <li v-for="Banneritem in Bannerlist" v-bind:key="Banneritem.id">  <a href="#"><img :src="require(`../assets/img/${Banneritem.image}`)" alt="">{{Banneritem.label}}</a></li>
                    
                </ul>
            </div>
        </div>
    </div>
</template>



<script>
export default {
  name: 'C3',
  components:{},
      data() {
        return {
            Bannerlist: [
                { label: 'DIGITAL COMICS', image: 'buy-comics-digital-comics.png' },
                { label: 'DC MERCHANDISE', image: 'buy-comics-merchandise.png' },
                { label: 'SUBSCRIPTION', image: 'buy-comics-subscriptions.png' },
                { label: 'COMIC SHOP LOCATOR', image: 'buy-comics-shop-locator.png' },
                { label: 'DC POWER VISA', image: 'buy-dc-power-visa.svg' },
            ]
        };
    },
  props: {
    msg: String
  }
}
</script>



<style scoped lang="scss">
@import '../assets/scss/variables.scss';
.box-C3{
    @include layout-block-1;
}
.layout-box{
    @include layout-block-1;

    background-color: $sie-color-2;
}
.centered-box{
    @include layout-block-2;
    justify-content: space-between;
}
#banner-list > li > a img{
    width: 100px;
}
</style>
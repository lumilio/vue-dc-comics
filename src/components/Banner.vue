<template>
    <div class="box-C3">
        <div class="layout-box">
            <div class="centered-box">
                <ul id='banner-list'>
                    <Icon v-for="Banneritem in Bannerlist" v-bind:key="Banneritem.id" :image="Banneritem.image" :label='Banneritem.label'/>  
                </ul>
            </div>
        </div>
    </div>
</template>



<script>

import Icon from './IconBannerModel.vue'

export default {
  name: 'C3',
  components:{
      Icon,
  },
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
    z-index: 1;
}
.centered-box{
    @include layout-block-2;
}
#banner-list{
    padding: 0;
    display: flex;
    margin: 30px 0;
    justify-content: space-between;
    width: 100%;
}
</style>
<template>
    <div class="box-C5">
        <div class="layout-box">
            <div class="centered-box">
                <button>xxxx</button>
                <div>
                    <a href="#">FOLLOW US</a>
                    <ul id='header-list'>
                        <li v-for="link in links" v-bind:key="link.id"> <a href="#"><img :src="require(`../assets/img/${link}`)" alt=""></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>



<script>
export default {
  name: 'C5',
  components:{},
    data() {
        return {
            links: [
                'footer-facebook.png',
                'footer-twitter.png',
                'footer-youtube.png',
                'footer-pinterest.png',
                'footer-periscope.png',
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
.box-C1{
    @include layout-block-1;
}
.layout-box{
    @include layout-block-1;
    background-color: #303030;
    z-index: 1;
}
.centered-box{
    @include layout-block-2;
    justify-content: space-between;
}
#header-logo{
    width: 67px;
    height: 67px;
}
#header-list{
    margin: 0;
}
#header-list li{
    display: inline-block;
    margin: 0 14px;
}
#header-list a{
    text-decoration: none;
    font-size: 11px;
    line-height: 85px;
    color: $sie-color-1;
}
#header-list li:hover{
    border-bottom: 5px solid $sie-color-2;
}
#header-list li:hover > a{
    color: $sie-color-2;
}
</style>
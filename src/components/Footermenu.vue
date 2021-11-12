<template>
    <div class="box-C5">
        <div class="layout-box">
            <div class="centered-box">
                <button>SING-UP NOW!</button>
                <div class="follow-links">
                    <a id='followtag' href="#"><b>FOLLOW US</b></a>
                    <ul id='footer-list'>
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
.box-C5{
    @include layout-block-1;
    z-index: 100;
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
.centered-box button{
    padding: 10px;
    color: white;
    border: 1px solid $sie-color-2;
    background-color: #303030; 
}
.centered-box button:hover{
    background-color: $sie-color-2; 
    cursor: pointer;
}
#footer-list{
    margin: 27px 0;
}
#footer-list li{
    display: inline-block;
    margin: 0 8px;
}
#footer-list a img{
    width: 27px;
}
.follow-links{
    display: flex;
    align-items: center;
}
#followtag{
    text-decoration: none;
    color: $sie-color-2;
}
</style>
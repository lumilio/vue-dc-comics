<template>
    <div class="box-C4">
        <div class="layout-box">
            <div class="centered-box">
                <div>
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li>ss</li>
                            <li>ssss</li>
                            <li>ssss</li>
                            <li>ss</li>
                            <li>sss</li>
                            <li>sss</li>
                            <li>ss</li>
                        </ul>
                    </div>
                    <div>
                        <h3>SHOP</h3>
                        <ul>
                            <li>ss</li>
                            <li>ssss</li>
                            <li>ssss</li>
                            <li>ss</li>
                            <li>sss</li>
                            <li>sss</li>
                            <li>ss</li>
                        </ul>
                    </div>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                    </ul>
                </div>
                <div>
                    <h3>SITES</h3>
                    <ul>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                        <li>ss</li>
                    </ul>
                </div>
                <img id='footer-logo' src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>



<script>
export default {
  name: 'C1',
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
.box-C1{
    @include layout-block-1;

}
.layout-box{
    @include layout-block-1;
    background-image: url('../assets/img/footer-bg.jpg') ;
    background-position-y: top;
    background-position-x: center;
    background-size: cover;
    /* background-repeat: no-repeat */
    z-index: -2
}
.centered-box{
    width: 1140px;
    display: flex;
    position: relative;
    height: 500px;
    color: white;
}
.centered-box img{
    position: absolute;
    right: 0;
    top: -95px;

}

</style>


<template>
    <div class="box-C4">
        <div class="layout-box">
            <div class="centered-box">
                <div class="mini-list">
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                    </div>
                    <div>
                        <h3>SHOP</h3>
                        <ul>
                            <li><a href="#">Shop DC</a> </li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                </div>
                <div class="mini-list">
                    <h3>DC</h3>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshop</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="mini-list">
                    <h3>SITES</h3>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
                <img id='footer-logo' src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>



<script>
export default {
  name: 'C4',
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
.layout-box{
    @include layout-block-1;
    background-image: url('../assets/img/footer-bg.jpg') ;
    background-position-y: top;
    background-position-x: center;
    background-size: cover;
    /* background-repeat: no-repeat */
}
.centered-box{
    width: 1140px;
    display: flex;
    position: relative;
    color: white;
}
.mini-list{
    margin: 30px 70px 62px 0px;
}
.centered-box h3{
    margin-bottom: 0;
}
.centered-box ul{
    padding: 0;
    margin-top: 10px;
    list-style: none;
}
.centered-box li a{
    color: #636b6b;
    text-decoration: none;
    font-size: smaller;
}
.centered-box li a:hover{
    color: #abb5b5;
    text-decoration: underline;
}
.centered-box img{
    position: absolute;
    right: 0;
    top: -95px;
}
</style>


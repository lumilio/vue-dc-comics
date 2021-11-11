<template>
    <div class="box-C1">
        <div class="layout-box">
            <div class="centered-box">
                <img id='header-logo' src="../assets/img/dc-logo.png" alt="">
                <ul id='header-list'>
                    <li v-for="Menuitem in Menulist" v-bind:key="Menuitem"> <a href="#">{{Menuitem}}</a></li>
                </ul>
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
            Menulist: ['CHARACTERS','COMICS','MOVIES','TV','GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS','SHOP',]
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
    margin-top: 1rem;
    background-color: white;
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
    border-top: 5px solid white;
    border-bottom: 5px solid white;
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
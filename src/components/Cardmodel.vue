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
</style>
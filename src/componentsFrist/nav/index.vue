<template>
  <div>
 <div class="tab_mask" v-if="isShow"  >
        <h3>全部频道</h3>
        <ul class="nav_mask_list" >
            <li class="nav_mask_item"  v-for="(e,i) in Data" :key="i">
                {{e}}
            </li>
 

        </ul>
</div>
       <div class="first_nav" ref="nav">
        <ul class="nav_list" >
            <li class="nav_item " :class="{active:i-0===isIndex}" v-for="(e,i) in Data" :key="i" @click="active(i)" >{{e}}</li>

        </ul>
        <span class="iconfont" id="menuBtn"  @click="isShow=!isShow" ><img   src="./img/下箭头.png"  ></span>
     </div>
  </div>
</template>

<script type="text/ecmascript-6">
  import Bscroll from 'better-scroll'
  export default {
    props:['Data'],
    data(){
      return{
        isShow:false,
        isIndex:0
      }
    },
    mounted(){
      let nav_list = this.$refs.nav
      new Bscroll(nav_list,{
        scrollX:true
      })
     
    },
    methods:{
        active(index){
          this.isIndex=index
        }
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>

   .tab_mask //导航msk
    position absolute
    left 0rem
    top 2.3rem //2
    z-index 5
    width 100%
    background white
    h3
      height 2.5rem
    .nav_mask_list
      box-sizing border-box
      width 100%
      display flex
      flex-wrap wrap
      .nav_mask_item
       display flex
       align-items center
       justify-content space-around
       width 20%
       height 1rem
       border 0.3rem solid #ccc
       background #eeeeee
       margin 0.5%
       font-size 0.5rem
       text-align center
       line-height 0.5rem
  .first_nav
    position relative
    //padding-top  2.2rem
    box-sizing border-box
    padding-top 0.65rem
    overflow hidden
    height 2.2rem

    span
      position absolute
      right 0rem
      top 0rem
      z-index 10
      text-align center
      font-size 2rem
      line-height 2rem
      width 4rem
      height 2.2rem
      background white
    .nav_list
      width 215%
      font-size 0.5rem
      padding 0.2rem
      .nav_item
        display inline-block
        padding 0 0.2rem
        text-align center
        font-size 0.5rem
        line-height 0.5rem
        width 3rem
       & .active
         color red
         border-bottom 1px solid red
</style>

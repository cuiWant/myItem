<template>
<div class="frist_newperson recommend" id="recommend">
            <div class="brand_header">
                <span class="left_text">人气推荐</span>
                <span class="right_text"> 更多》</span>
            </div>
            <div class="recommend_top" >
                <img src="https://yanxuan-item.nosdn.127.net/89d86a4e463115e366daf841b9bcff46.png?imageView&quality=65&thumbnail=280x280" alt="">
                <div class="recommend_top_text">
                    <span class="recommend_top_text_title .border-1px">超低优惠</span>
                    <h4 class="h4">新色 奢华植鞣头层水牛皮席 凉席三件套</h4>
                    <span class="statement">三峡水牛头层皮，高端夏凉必备</span>
                    <span class="recommend_top_text_prise">￥1949</span>
                </div>
            </div>
            <div class="recommend_bottom">
                <ul class="recommend_bottom_list">
                    <li class="recommend_bottom_item">
                        <div class="recommend_bottom_item_content">
                            <img src="https://yanxuan.nosdn.127.net/d2abd30e0296cdee86f1bdd9242c0937.png?imageView&quality=65&thumbnail=330x330" alt="">
                        </div>
                        <div class="recommend_bottom_item_text">
                       <span>
                           风驰电掣 大运摩托
                            风驰电掣 大运摩托
                        </span>
                            <span class="red_prise">
                                ￥199
                            </span>
                        </div>
                        <div class="red_prise_footer">
                            <span>加价购</span>
                        </div>
                    </li>
                    <li class="recommend_bottom_item">
                        <div class="recommend_bottom_item_content">
                            <img src="https://yanxuan-item.nosdn.127.net/ffaaa0b99d13210e8adc7d81176a53f8.png?imageView&quality=65&thumbnail=330x330" alt="">
                        </div>
                        <div class="recommend_bottom_item_text">
                       <span>
                           男式全棉干爽型宽松短袖T恤...
                        </span>
                            <span class="red_prise">
                                ￥47.4
                            </span>
                        </div>
                        <div class="red_prise_footer">
                            <span>季末特惠</span>
                        </div>
                    </li>
                    <li class="recommend_bottom_item">
                        <div class="recommend_bottom_item_content">
                            <img src="https://yanxuan-item.nosdn.127.net/e5474a8f4fd5748079e2ba2ead806b51.png?imageView&quality=65&thumbnail=330x330" alt="">
                        </div>
                        <div class="recommend_bottom_item_text">
                       <span>
                    日式和风声波式电动牙刷（可...
                        </span>
                            <span class="red_prise">
                                ￥129
                            </span>
                        </div>
                        <div class="red_prise_footer">
                            <span>满减</span>
                        </div>
                    </li>
             </ul>
            </div>

        </div>
</template>

<script type="text/ecmascript-6">
  export default {
  }
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
   .recommend
     width 100%
     .recommend_top
       width 100%
       background darkkhaki
       height 4rem
       img
        display inline-block
        width 40%
        height 4rem
       .recommend_top_text
         height 100%
         display flex
         flex-direction column
         justify-content center
         width: 60%
         float right
         h4
          font-size 0.5rem
          font-weight 700
          white-space nowrap
          overflow:hidden;
          text-overflow:ellipsis
        .statement
          font-size 0.4rem
          color #eee
        .recommend_top_text_title
          height 0.5rem
          padding 0.1 rem
          background white
          text-align center
          line-height 0.3rem
          font-size 0.3rem
          width 2rem
          color red
          border 1px solid red
        .recommend_top_text_prise
          font-size 0.5rem
          color red
      .recommend_bottom
        height 5rem
        width 100%
        .recommend_bottom_list
          width 100%
          display  flex
          justify-content space-between
          margin-top 0.1rem
          .recommend_bottom_item
            width 30%
            display flex
            align-items center
            flex-direction column
            .recommend_bottom_item_content
              background wheat
              img
                width 100%
                height 3rem
            .recommend_bottom_item_text
              span
                font-size 0.3rem
                float left
               .red_prise
                  color red
            .red_prise_footer
              width 100%
              height 1rem
              font-size 0.4rem
              span
                text-align center
                line-height 0.4rem
                color pink
                border 1px solid #000

     .brand_header
      overflow hidden
      .left_text
        float left
       .right_text
         float right
</style>

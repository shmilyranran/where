<template>
    <div>
      <div class="recommend-title">
        周末去哪儿
      </div>
      <ul>
     <li class="item border-bottom" v-for="item in recommendList" :key="item.id">
         <div class="item-img-wrapper">
             <img class="item-img" :src="item.imgUrl"/>
         </div>
         <div class="item-info">
         <p class="item-title">{{item.title}}</p>
         <p class="item-desc">{{item.desc}}</p>
          </div>
         </li>    
      </ul>
    </div>
</template>

<script>
    export default {
        name:"HomeWeekend",
        data(){
            return{
                recommendList:[{
                    id:'0001',
                    imgUrl:'http://img1.qunarzz.com/piao/fusion/1712/91/a275569091681d02.jpg_640x200_0519ccb9.jpg',
                    title:"大连圣亚海洋世界",
                    desc:"浪漫大连首站，浪漫的海洋主题乐园"
                },{
                    id:'0002',
                    imgUrl:'http://img1.qunarzz.com/piao/fusion/1712/91/a275569091681d02.jpg_640x200_0519ccb9.jpg',
                    title:"大连圣亚海洋世界",
                    desc:"浪漫大连首站，浪漫的海洋主题乐园"
                },{
                    id:'0003',
                    imgUrl:'http://img1.qunarzz.com/piao/fusion/1712/91/a275569091681d02.jpg_640x200_0519ccb9.jpg',
                    title:"大连圣亚海洋世界",
                    desc:"浪漫大连首站，浪漫的海洋主题乐园"
                }]
            }
        }
    }
</script>

<style lang="stylus" scoped>
@import '~@/assets/mixins.styl'
   .recommend-title
     marign-top:.2rem
     line-height:.8rem
     background:#eee
     text-indent:.2rem
   .item-img-wrapper
      overflow:hidden
      height:0
      padding-bottom:33.9%
    .item-img
      width:100%
   .item-info
       
       padding:0.1rem
      
   .item-title
       list-height:0.54rem
       font-size:0.32rem
       ellipsis()
   .item-desc
       line-height:.4rem
       color:#ccc
       ellipsis()

</style>
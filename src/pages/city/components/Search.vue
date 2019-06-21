<template>
    <div class="search">
     <input type="text" class="search-input" placeholder="输入城市名或拼音"/>
    </div>
</template>

<script>
    export default {
        name:"CitySearch"
    }
</script>

<style lang="stylus" scoped>
@import '~@/assets/varibles.styl'
.search
 height:.72rem
 background:$bgColor
 padding:0 .1rem
.search-input 
    box-sizing:border-box
    height:.62rem
    list-height:.62rem
    padding:0 .1rem
    text-align:center
    border-radius:.06rem
    width:100%
    color:#666
</style>
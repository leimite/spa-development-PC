<template>
    <div class="sass-wrap">
      <div>sass简易使用</div>

    <div class="test-sass">
      sass测试容器 sass测试容器 sass测试容器 sass测试容器
    </div>
    </div>

</template>

<script type="text/javascript">

  export default {
     name: 'page1'
  }
</script>

<style lang="scss" scoped>
  @import "~assets/css/variable";
  @import "~assets/css/mixin";
  /*SASS的常用变量 宏 已定义在assets/css/variable  mixin里*/
  .test-sass{
    width: 200px;
    height: 100px;
    margin: 0 auto;
    /*使用SASS变量*/
    color:$cl-txt;
    /*使用SASS宏命令*/
    @include no-wrap
  }

</style>

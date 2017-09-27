<template>
  <div >
    <!--<image class="img" :src="src"></image>-->
    <!--<TopHeader></TopHeader>-->
    <!--<hello></hello>-->
    <!--<Test></Test>-->
    <!--<lh-video-stream class="lh-liveStream" url="rtmp://live.hkstv.hk.lxdns.com/live/hks">-->
      <!--<div>-->
        <!--<text>asdasdasdasd</text>-->
      <!--</div>-->
      <!--<div>-->
        <!--<text>asfeghtehe</text>-->
      <!--</div>-->
    <!--</lh-video-stream>-->
  </div>
</template>

<script>
//import Hello from './components/Hello.vue'
//import TopHeader from './components/TopHeader.vue'
import Test from './components/Test.vue'
var modal=weex.requireModule('modal');

export default {
  name: 'app',
//  created () {
//      modal.toast({
//          message:'页面加载成功',
//          duration:3
//      })
//  },
  data () {
    return {
      src: "https://img.alicdn.com/tfs/TB1OOl1SVXXXXc_XVXXXXXXXXXX-340-340.png"
    }
  },
  components: {
//    Hello,
      Test
//      TopHeader
  }
}
</script>

<style scoped>
.app {
  align-items: center;
  padding-top: 200px;
}
.img {
  width: 340px;
  height: 340px;
}
.lh-liveStream {
  width: 460px;
  height:720px;
}
</style>

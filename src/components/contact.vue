<template>
      <div class="myconnect">
          <a href="http://github.com/nopapername/vue-resume" target="_blank" class="iconfont" id="github" data-toggle="tooltip" data-placement="bottom" :title="github">&#xe6f6;</a>
          <a href="#" class="iconfont" id="weixin" data-toggle="tooltip" data-placement="bottom" :title="weixin" data-html="true">&#xe654;</a>
          <a href="#" class="iconfont" id="qq" data-toggle="tooltip" data-placement="bottom" :title="qq" data-html="true">&#xe66a;</a>
          <a href="https://weibo.com/u/6020961867?topnav=1&wvr=6&topsug=1" target="_blank" class="iconfont" id="weibo" data-toggle="tooltip" data-placement="bottom" :title="weibo">&#xe66b;</a>
          <a href="https://blog.csdn.net/weixin_43388844" target="_blank" class="iconfont" id="csdn" data-toggle="tooltip" data-placement="bottom" :title="csdn">&#xe600;</a>
        </div>
</template>>
<style scoped>
.myconnect {
  width: 110%;
  position: relative;
  right: 48px;
}
a {
  text-decoration: none;
  color: black;
}
.iconfont {
  margin-left: 50px;
  font-size: 40px;
  cursor: pointer;
}
.myconnect a:nth-child(1):hover {
  color: rgb(65, 65, 65);
}
.myconnect a:nth-child(2):hover {
  color: rgb(13, 161, 0);
}
.myconnect a:nth-child(3):hover {
  color: rgb(0, 132, 255);
}
.myconnect a:nth-child(4):hover {
  color: rgb(118, 0, 165);
}
.myconnect a:nth-child(5):hover {
  color: rgb(197, 13, 0);
}
</style>>
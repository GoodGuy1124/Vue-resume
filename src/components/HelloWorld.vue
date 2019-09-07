<template>
<div>
<div class="hello" v-show="!showoff">
  <div class="head">
    <span class="lg" @mouseenter="addcardAnimate"  @mouseleave="delcardAnimate" :class="cardani">正致力于成为一名合格的前端工程师</span>
     <vue-particles
        color="#fff"
        :particleOpacity="0.7"
        :particlesNumber="60"
        shapeType="circle"
        :particleSize="4"
        linesColor="#fff"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="2"
        :hoverEffect="true"
        hoverMode="grab"
        :clickEffect="false"
        clickMode="push"
        class="lizi"
      >
      </vue-particles>
  </div>
  <div class="continer" >
    <div class="box animated bounceInDown" >
      <div class="center-topbox">
      <div class="outer">
        <div class="inner">神秘面纱</div>
      </div>
      <div class="right-box">
      <span class="myword">拥有较强的自学能力，热爱编程，乐于学习最新前沿技术，努力提升自己，能独立解决项目中遇到的问题，拥有表达沟通能力能适应各种环境，并融入其中，为人乐观开朗，喜欢与人相交，并虚心向他人学习，善于总结，也乐于向他人分享自己所得经验，工作中认真负责，力求完美，尽力在规定时间内完成规定内容并保证项目质量。
</span>
      </div>
      <skill class="skill"></skill>
      <works></works>
     <!-- <contact></contact> -->

    </div></div>
    <div class="left">
      <ul class="left-ul">
        <li><img src="../assets/xueli.png"/><span>本科</span></li>
        <li><img src="../assets/years.png"/><span>22岁</span></li>
        <li><img src="../assets/adrss.png"/><span>成都</span></li>
        <li><img src="../assets/zhuangye.png"/><span>软件技术</span></li>
        <li><img src="../assets/tel.png"/><span>15730332797</span></li>
        <li><img src="../assets/email.png"/><span class="email">986352872@qq.com</span></li>
        <li></li>
      </ul>
    </div>
    <div class="right">
      <timeline></timeline>

    </div>
    
    </div>
      <a class="my-head" href="www.baidu.com">
        <img src="../assets/headP.jpg">
        <h5>GoodGuy</h5>
        <h6><span>陈卓</span> 's resume</h6>
      </a>
	</div>
  <phonepage v-show="showoff"></phonepage>
  </div>

</template>

<script>
import skill from '../components/skills'
import works from '../components/works'
import timeline from '../components/timeline'
import phonepage from '../components/phonepage'
import contact from '../components/contact'
export default {
  created(){
    console.log("here");
     var  that=this;
            window.onresize = function temp() {
               console.log(`${document.documentElement.clientWidth*0.4}`);
              if(`${document.documentElement.clientWidth*0.4}`<700){
               
              that.showoff=true
              }else{
                that.showoff=false
              }
                // that.styleObject.height = `${document.documentElement.clientWidth*0.4}px`;
            };
  },
  data () {
    return {
      cardani: '',
      showoff:false,
      styleObject: {
                    height: '900px'
                }
    }
  },
  mounted() {
          var  that=this
            window.onresize = function temp() {
              if(`${document.documentElement.clientWidth*0.4}`<400){
              that.showoff=true
              }else{
                that.showoff=false
              }
                // that.styleObject.height = `${document.documentElement.clientWidth*0.4}px`;
            };
        },
  methods: {
       addcardAnimate () {
      this.cardani = 'heartBeat'
    },
    delcardAnimate () {
      this.cardani = ''
    }
},
components: {
  skill,
  works,
  timeline,
  phonepage,
  contact

}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body{
  min-width:1000px; 
}
.email{
  font-size: 15px;
}
  .left-ul{
    list-style: none;
    line-height: 40px;
    margin-left: -20px;
     /* vertical-align: middle */
  }
  .left-ul img{
    width: 20px;
    height: 20px;
    vertical-align: middle
  }
  .left-ul span{
    margin-left: 5px;
  }
   .my-head{
       display: block;
       width: 230px;
       height: 70px;
       background-color: rgba(155, 155, 155, 0.5);
       top: 5%;
       right: 2%;
       border-radius: 15px;
       cursor: pointer;
       color: black;
       text-decoration: none;   
       position: fixed;

   }
   .my-head:hover {
  color: black;
  text-decoration: none;
}
.my-head img {
  position: relative;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin: 10px;
}
.my-head h5 {
  position: absolute;
  top: 0px;
  left: 70px;
}
.my-head h6 {
  position: absolute;
  top: 17px;
  left: 80px;
  color: black;
}
.my-head span {
  padding: 0 8px;
  border-radius: 5px;
  background-color: black;
  color: white;
}
.my-head p {
  padding: 0;
  margin: 0;
}
  .center-topbox{
    width: 100%;
    height: 172px;
    /* background: green; */
    border-bottom-width: 3px;
    border-bottom-color: cornflowerblue;
    border-bottom-style: solid;
    

  }
  .right-box{
     width: 70%;
    height: 172px;
    display: inline-block;
    font-family: 'Courier New', Courier, monospace;
    font-size: 20px;
    /* word-break: break-all; */
    vertical-align:middle;
    overflow: hidden;
   }
    .myword{
      width: 100%;
      height: 152px;
      margin-top: 10px;
      /* background: black; */
      color: white;
      line-height:35px;
    }
       .outer{
         margin-left: 20px;
       }
	.outer,.inner{
    vertical-align:middle;
				height: 172px;
				width: 150px;
        display: inline-block;
				background-image: url('../assets/head1.png');
       
			}
	.inner{
				background: hotpink;
				transition: all 1s;
				transform-origin: left top;
        opacity: 0.8;
			}
			
	.inner:hover{
				transform: rotate(90deg);
			}
  .hello {
       width: 100%;
       height: 100vh;
    }
    .head{
      width: 100%;
      height: 200px;
      overflow: hidden;
      background-color:black;
      
    }
    .lg{
      color: rgb(255, 255, 255);
      font-size: 25px;
      font-family: 'STKaiti','Courier New', Courier, monospace;
      position: absolute;
      margin-top: 100px;
      margin-left: 35%;

    }
     .continer{
	  height:1000px;
	  padding:0 180px 0 200px;
    background-color: #FFF8DC;
	  }
  .box{
	  width:100%;
	  height:100%;
	  background-color:#EECBAD;
	  float:left;
	  }
  .left{
	  width:200px;
	  height:100%;
	  float:left;
	  position:relative;
	  margin-left:-100%;
	  left:-200px;
    
	  }
   .right{
    float:left;
    width:180px;
    height:100%;
    margin-left:-180px;
    /*中间栏的位置摆正之后，右栏的位置也相应左移，通过相对定位的right恢复到正确位置*/
    position:relative;
    right:-180px;
   
	  }


</style>

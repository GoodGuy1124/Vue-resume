<template>
     <div class="page animated zoomIn">
      <div class="continar-head">
          <img src="../assets/headP.jpg">
          <h3 class="logoname">GoodGuy's resume</h3>
      </div>
      <div class="aboutme">
        <h3>AboutMe</h3>
        <p>
          您好,我叫陈卓，坐标重庆。我是重庆人文科技学院软件技术专业2016级大四的学生，有着一定的编程基础，目前能够熟练使用Html、Css、Javascript等前端Web开发技术，熟悉jquery、ElementuI框架、Vue框架等的基础,能基本使用webpack、npm、git等工具,对前端很感兴趣，具有良好的自学能力，目前的规划是先找一份实习工作磨砺自我，积累工作经验，学习更多前端相关知识，想要学习一些后端相关知识以更好的应对前端各种工作，努力的成为一名合格的前端工程师！
        </p>
      </div>
    <div class="skills">
        <h3>Skills mastered</h3>
        <ul>
        <li><div style="background:#C96300">Vue.js</div><p style="width:50%; background:#FF8817"></p></li>
        <li><div style="background:#0F5487">Html Css</div><p style="width:50%; background:#177FCB"></p></li>
        <li><div style="background:#F0B109">JavaScript</div><p style="width:50%; background:#F8CA4D"></p></li>
        <li><div style="background:#3D4670">Java</div><p style="width:30%; background:#5864A2"></p></li>
        <li><div style="background:#BA437D"> Android</div><p style="width:30%; background:#CF7AA4"></p></li>
        <li><div style="background:#475050">ElementUI</div><p style="width:40%; background:#B2CACA"></p></li>
        
    </ul>
      </div>
      <div class="works">
          <h3>MyWorks</h3>
          <works></works>

      </div>

     </div>
</template>
<script>
import works from '../components/works'
export default {

    components: {
 
  works,
  
}

}

</script>>

<style scoped>
ul li p{
   
    height: 100%;
    position: absolute;
    left:84px;
    top:-16px;
}

ul{
    display: inline-block;
    width: 70%;
    height: 300px;
    /* background: violet; */
    overflow: hidden;
    vertical-align:middle;
}
ul li {
    background:white;
    list-style: none;
    margin-top: 20px;
    border: 1px solid teal;
    border-radius: 10%;
    position: relative;

}
ul li div{
    width: 80px;
    background: salmon;
    border: 2px solid teal;
    color:seashell;
}
.works h3{
  width: 100px;
  position: relative;
  left: 50%;
  margin-left: -50px;
  border-bottom: 2px solid blueviolet;

}
.skills h3{
  width: 150px;
  position: relative;
  left: 50%;
  margin-left: -75px;
  border-bottom: 2px solid blueviolet;
}
.aboutme h3 {
  width: 90px;
  position: relative;
  left: 50%;
  margin-left: -45px;
  border-bottom: 2px solid blueviolet;
 
}
.aboutme p {
    padding: 10px;
    line-height: 30px;
}

.logoname{
      width: 200px;
      height: 40px;
      position: absolute;
      bottom:10px;
      left:50%;
       margin-left: -100px;
}
img{
    width: 100px;
    height: 100px;
    border-radius: 50%;
    position: absolute;
    top:10px;
    left:50%;
    margin-left: -50px;
    
}
.continar-head{
    width: 100%;
    height: 200px;
    background: #A4D3EE;
    position: relative;
}

</style>
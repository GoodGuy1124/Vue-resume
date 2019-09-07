<template>
    <ul >
        <li >至今</li>
        <li >2018.9</li>
        <li >2017.10</li>
        <li >2016.10</li>
        <li >2015.9</li>
        <div class="experience">
        <div >正在找工作</div>
        <div >参加重庆专升本考试，进入本科院校(重庆人文科技学院)学习</div>
        <div>参加MIAC应用挑战赛国赛获得一等奖(Android方面)</div>
        <div>加入学校工作室负责前端开发</div>
        <div >进入重庆工程职业技术学院学习</div>
        </div>
    </ul>
       <!-- <ul >
        <li @mouseover="showoff(1)" @mouseleave="showup(1)">至今</li>
        <li @mouseover="showoff(2)" @mouseleave="showup(2)">2018.9</li>
        <li @mouseover="showoff(3)" @mouseleave="showup(3)">2017.10</li>
        <li @mouseover="showoff(4)" @mouseleave="showup(4)">2016.10</li>
        <li @mouseover="showoff(5)" @mouseleave="showup(5)">2015.9</li>
        <div class="experience">
        <div v-show="IsShow1">正在找工作</div>
        <div v-show="IsShow2">参加重庆专升本考试，进入本科院校(重庆人文科技学院)学习</div>
        <div v-show="IsShow3">参加MIAC应用挑战赛国赛获得一等奖(Android方面)</div>
        <div v-show="IsShow4">加入学校工作室负责前端开发</div>
        <div v-show="IsShow5">进入重庆工程职业技术学院学习</div>
        </div>
    </ul> -->
</template>
<script>
export default {
  data () {
    return {
    //  IsShow1:false,
    //  IsShow2:false,
    //  IsShow3:false,
    //  IsShow4:false,
    //  IsShow5:false,
    }
  },
  methods: {
      
    //   showoff(count){
          
    //       if(count==1){this.IsShow1=true}
    //       else if(count==2){this.IsShow2=true}
    //       else if(count==3){this.IsShow3=true}
    //       else if(count==4){this.IsShow4=true}
    //       else if(count==5){this.IsShow5=true}
         
       
    //   },
    //   showup(counts){
    //       if(counts==1){this.IsShow1=false}
    //       else if(counts==2){this.IsShow2=false}
    //       else if(counts==3){this.IsShow3=false}
    //       else if(counts==4){this.IsShow4=false}
    //       else if(counts==5){this.IsShow5=false}

    //   }

},

}
</script>>
<style scoped>

ul{
    /* list-style: none; */
    width: 50px;
    height: 100%;
    background: #C1FFC1;
    margin: auto;
    position: relative;
    border: 1px solid aqua;
    border-radius: 5px;
}
li{
    list-style: none;
    width: 100%;
    height: 30px;
    position: absolute;
    left: 0px;
    text-align: center;
    cursor: pointer;
    
}
li:nth-child(2),.experience div:nth-child(2){
    top:20%;
}
li:nth-child(3),.experience div:nth-child(3){
    top:40%;
}
li:nth-child(4),.experience div:nth-child(4){
    top:60%;
    
}
li:nth-child(5),.experience div:nth-child(5){
    top:80%;
}

li:nth-child(1):hover~.experience div:nth-child(1) {
    opacity:0.8 ;
    
   
}
ul li:nth-child(2):hover~.experience div:nth-child(2){
   opacity: 0.8;
    
} 
ul li:nth-child(3):hover~.experience div:nth-child(3){
   opacity: 0.8;
    
}
ul li:nth-child(4):hover~.experience div:nth-child(4){
    opacity: 0.8;
    
}
ul li:nth-child(5):hover~.experience div:nth-child(5){
  opacity: 0.8;
    
}

.experience div{
    width: 200px;
    height: 100px;
    background: yellowgreen;
     position: absolute;
     font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
     font-weight: 10px;
     line-height: 30px;
     left:-200px;
     opacity: 0;
     border-radius: 10%;
     transition: all 1s;
}

</style>>
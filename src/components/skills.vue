<template>
<div class="contiar">

    <h5>技能栈</h5>
    <ul>
        <li><div style="background:#C96300">Vue.js</div><p style="width:60%; background:#FF8817"></p></li>
        <li><div style="background:#0F5487">Html Css</div><p style="width:70%; background:#177FCB"></p></li>
        <li><div style="background:#F0B109">JavaScript</div><p style="width:60%; background:#F8CA4D"></p></li>
        <li><div style="background:#3D4670">Java</div><p style="width:40%; background:#5864A2"></p></li>
        <li><div style="background:#BA437D"> Android</div><p style="width:40%; background:#CF7AA4"></p></li>
        <li><div style="background:#475050">ElementUI</div><p style="width:60%; background:#B2CACA"></p></li>
        
    </ul>

</div>
</template>
<style scoped>
.contiar{
    border-bottom-width: 3px;
    border-bottom-color: cornflowerblue;
    border-bottom-style: solid;
}
ul li p{
   
    height: 100%;
    position: absolute;
    left:84px;
    top:-16px;
}
h5{
    display: inline-block;
    vertical-align: middle;
    word-break: break-all;
    margin: 20px;
    width: 40px;
    word-wrap: break-word;
    font-size: 24px;
    
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

</style>
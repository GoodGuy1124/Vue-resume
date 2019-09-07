<template>

    <div class="bigcont">
   <div class="cont">
			
			<img src="../assets/Hydrangeas.jpg" >
		
			<img src="../assets/Penguins.jpg" >
			
			<img src="../assets/Koala.jpg" >
			<img src="../assets/Tulips.jpg" >
				<img src="../assets/Lighthouse.jpg" >
			<img src="../assets/Jellyfish.jpg" >
			<div class="sm-box">
				<div class="box"></div>
				<div class="box"></div>
				<div class="box"></div>
				<div class="box"></div>
				<div class="box"></div>
				<div class="box"></div>
			</div>
		</div>
    </div>
</template>>
	
		<style scoped>
        
      .bigcont{
		        border-bottom-width: 3px;
                border-bottom-color: cornflowerblue;
                border-bottom-style: solid;
	  }
		.cont{
				width: 300px;
				height: 300px;
				position: relative;
				transition: all 2s;
				transform-style: preserve-3d;
				/* perspective: 2000px; */
				margin: auto;
				transform-origin: center center 150px;
				animation: move 5s;
				animation-iteration-count: infinite;
			}
			.cont img{
				width: 100%;
				height: 100%;
				position: absolute;
				top: 0;
				left: 0;
				opacity: 0.9;
				transition: all 1s;
			}
			.sm-box{
				width: 100px;
				height: 100px;
				
				position: absolute;
				top: 100px;
				left: 100px;
				transform-style: preserve-3d;
				/* perspective: 2000px; */
				transform: translateZ(100px);
			}
			.box{
				width: 100%;
				height: 100%;
				position: absolute;
				top: 0;
				left: 0;
				background: url(../assets/user-photo.png);
				background-size:100% 100%;
			}
			.box:nth-child(1),
			img:nth-child(1){
				transform-origin: center top;
				transform: rotateX(90deg);
				z-index: 6;
			}
			.box:nth-child(2),
			img:nth-child(2){
				transform-origin: center bottom;
				transform: rotateX(-90deg);
				z-index: 5;
			}
			.box:nth-child(3),
			img:nth-child(3){
				transform-origin: left center;
				transform: rotateY(-90deg);
				z-index: 4;
			}
			.box:nth-child(4),
			img:nth-child(4){
				transform-origin: right center;
				transform: rotateY(90deg);
				z-index: 3;
			}
			.box:nth-child(5){
				transform: translateZ(100px);
				z-index: 2;
			}
			img:nth-child(5){
				transform: translateZ(300px);
				z-index: 2;
			}
			img:nth-child(6){
				transform: translateZ(0);
			}
			
			.cont:hover img:nth-child(1){
				transform:translateY(-100px) rotateX(90deg);
			}
			.cont:hover img:nth-child(2){
				transform:translateY(100px) rotateX(-90deg);
			}
			.cont:hover img:nth-child(3){
				transform:translateX(-100px) rotateY(-90deg);
			}
			.cont:hover img:nth-child(4){
				transform:translateX(100px) rotateY(90deg);
			}
			.cont:hover img:nth-child(5){
				transform:translateZ(400px)  ;
			}
			.cont:hover img:nth-child(6){
				transform:translateZ(-100px)  ;
			}
		
	
			@keyframes move{
				from{
					transform: rotateX(0) rotateY(0);
				}
				to{
					transform: rotateX(360deg) rotateY(360deg);
				}
			}
				
			
		</style>


	



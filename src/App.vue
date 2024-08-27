<script setup lang="ts">

// function openMailApplication() {
//   window.location.href = 'mailto:email@example.com'
// }
</script>

<template>
	<div class="portfolio_name">
		SZYMON CIURKIEWICZ
		<p style="font-size: 2vw; padding-top: 2vh;">scroll down 👇</p>
	</div>
	<div class="parallax">
    <div class="parallax__layer parallax__layer__0">
        <img src="./assets/1.svg" />
    </div>
    <div class="parallax__layer parallax__layer__1">
        <img src="./assets/2.svg" />
    </div>
    <div class="parallax__layer parallax__layer__2">
        <img src="./assets/3.svg" />
    </div>
    <div class="parallax__layer parallax__layer__3">
        <img src="./assets/4.svg" />
    </div>
    <div class="parallax__layer parallax__layer__4">
        <img src="./assets/5.svg" />
    </div>
    <div class="parallax__layer parallax__layer__5">
        <img src="./assets/6.svg" />
    </div>
    <div class="parallax__cover"></div>
</div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap');
* {
  box-sizing: border-box;
  
}

.portfolio_name {
	font-family: "Ubuntu", sans-serif;
	font-weight: 900;
	width: 100vw;
	height: 100vh;
	text-align: center; 
	vertical-align: middle; 
	font-size: 3vw;
	padding-top: 30vh;
}

html,
body {
  background-color: #ceddff;
  overflow-x: hidden; 
  overflow-y: auto;
}

.parallax {
  perspective: 100px;
  height: 100vh;
  overflow-x: hidden;
  overflow-y: auto;
  position: absolute;
  top: 0;
  left: 50%;
  right: 0;
  bottom: 0;
  margin-left: -1500px;
}

.parallax__layer {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}

.parallax__layer img {
  display: block;
  position: absolute;
  bottom: 0;
}

.parallax__cover {
  background: #00304a;
  display: block;
  position: absolute;
  top: 100%;
  left: 0;
  right: 0;
  height: 2000px;
  z-index: 2;
}

/* Translated from SCSS loop */
.parallax__layer__0 {
  transform: translateZ(-300px) scale(4);
}

.parallax__layer__1 {
  transform: translateZ(-250px) scale(3.5);
}

.parallax__layer__2 {
  transform: translateZ(-200px) scale(3);
}

.parallax__layer__3 {
  transform: translateZ(-150px) scale(2.5);
}

.parallax__layer__4 {
  transform: translateZ(-100px) scale(2);
}

.parallax__layer__5 {
  transform: translateZ(-50px) scale(1.5);
}

.parallax__layer__6 {
  transform: translateZ(0px) scale(1);
}

</style>
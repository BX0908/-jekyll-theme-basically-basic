---
layout: page
title: 音乐播放器
date: 2022-12-28
excerpt_separator: "<!--more-->"
categories:
     - svg制作
tags:
  - svg
---

循环播放的小小机器

<!--more-->
 <style>
	  body {
	    display: flex;
		width: 1200px;
		height: 800px;
	    justify-content: center;
	    align-items: center;
	    background: #FFA500;
	  }
	  .plinth {
	    background: #E1E1E1;
	    width: 300px;
	    height: 200px;
	    border-radius: 5px;
	    border: 5px solid #000;
	    display: flex;
	    align-items: center;
	    position: relative;
	  }
	  .adapter {
	    width: 25px;
	    height: 25px;
	    background: grey;
	    border-radius: 25px;
	    position: absolute;
	    top: 17.5px;
	    left: 8.5px;
	    display: flex;
	    justify-content: center;
	    align-items: center;
	  }
	  .innerAdapter {
	    width: 7px;
	    height: 7px;
	    background: black;
	    border-radius: 10px;
	  }
	  .strobe {
	    height: 20px;
	    width: 20px;
	    background: black;
	    border: 2px solid #c1c1c1;
	    border-radius: 20px;
	    position: absolute; 
	    bottom: 45px;
	    left: 5px;
	  }
	  .start {
	    width: 30px;
	    height: 20px;
	    background: #EAEAEA;
	    border: 4px inset #191919;
	    position: absolute;
	    bottom: 12.5px;
	    left: 2px;
	  }
	  .speedButton {
	    height: 5px;
	    width: 20px;
	    background: black;
	    position: absolute;
	    bottom: 15px;
	    left: 45px;
	    display: flex;
	  }
	  .thirtyThree {
	    width: 10px;
	    height: 5px;
	    background: #fff;
	    border: 1px solid #000;
	  }
	  .fortyFour {
	    width: 10px;
	    height: 5px;
	    background: #fff;
	    border: 1px solid #000;
	  }
	  .platterContainer {
	    width: 225px;
	    height: 180px;
	    background: #E1E1E1;
	  }
	  .platter {
	    width: 170px;
	    height: 170px;
	    border-radius: 180px;
	    border: 5px solid grey;
	    background: #3383FF;
	    margin: 0 auto;
	    position: relative;
	    display: flex;
	    justify-content: center;
	    align-items: center;
	  }
	  .record {
	    width: 160px;
	    height: 160px;
	    border-radius: 160px;
	    background: #191919;
	    display: flex;
	    align-items: center;
	    justify-content: center;
	    transform: rotate(0deg);
	    animation: 2s linear infinite nowPlaying;
	  }
	  .grooveLine {
	    height: 135px;
	    width: 135px;
	    border-radius: 135px;
	    background: #191919;
	    border: 2px double #000;
	    display: flex;
	    align-items: center;
	    justify-content: center;
	  }
	  .grooveInner {
	    height: 100px;
	    width: 100px;
	    background: #191919;
	    border: 2px double #000;
	    border-radius: 100px;
	    display: flex;
	    justify-content: center;
	    align-items: center;
	  }
	  .innerGroove {
	    height: 80px;
	    width: 80px;
	    background: black;
	    border-radius: 50px;
	  }
	  .label {
	    width: 60px;
	    height: 60px;
	    border-radius: 50px;
	    background: #000;
	    display: flex;
	    position: absolute;
	  }
	  .labelL {
	    width: 30px;
	    height: 60px;
	    border-radius: 60px 0 0 60px;
	    background: yellow;
	  }
	  .labelR {
	    width: 30px;
	    height: 60px; 
	    border-radius: 0 60px 60px 0;
	    background: green;
	  }
	  .spindle {
	    width: 10px;
	    height: 10px;
	    border-radius: 10px;
	    background: rgb(183, 183, 183);
	    position: absolute;
	  }
	  .rightSide {
	    width: 75px;
	    height: 180px;
	    background: #E1E1E1;
	    display: flex;
	    flex-direction: column;
	    position: relative;
	    z-index: 1;
	  }
	  .arm {
	    height: 75px;
	    width: 10px;
	    position: relative;
	    background: #9d9b9b;
	    margin: 0 auto;
	    border-radius: 0 0 0 50px;
	    transform-origin: top right 100%;
	    transform: translateX(-25px) translateY(15px) rotate(45deg);
	  }
	  .armBase {
	    height: 45px;
	    width: 45px;
	    border-radius: 100%;
	    background: #9d9b9b;
	    z-index: -1;
	    position: absolute;
	    top: 12.5px;
	    left: 4.5px;
	    display: flex;
	    justify-content: center;
	    align-items: center;
	  }
	  .innerBase {
	    height: 35px;
	    width: 35px;
	    border-radius: 35px;
	    background: black;
	  }
	  .counterWeight {
	    height: 25px;
	    width: 25px;
	    border-radius: 2px;
	    background: #DDDDDD;
	    border-top: 5px solid #222222;
	    border-bottom: 4px solid #222222;
	    position: absolute;
	    left: -7px;
	    top: -12.5px;
	    
	  }
	  .armBend {
	    height: 40px;
	    width: 10px;
	    border-radius: 50px 0 50px 0;
	    transform: rotate(-20deg);
	    background: #9d9b9b;
	    position: absolute;
	    bottom: -25px;
	    right: -5px;
	  }
	  .armBendTwo {
	    height: 40px;
	    width: 10px;
	    border-radius: 50px 50px 0 0;
	    transform: rotate(5deg);
	    background: #9d9b9b;
	    position: absolute;
	    bottom: -55px;
	    right: -8px;
	  }
	  .cartridge {
	    width: 16.5px;
	    height: 25px;
	    background: #000;
	    position: absolute;
	    bottom: -75px;
	    right: -8px;
	    transform: rotate(7deg);
	  }
	  .lift {
	    height: 5px;
	    width: 12.5px;
	    background: #fff;
	    position: absolute;
	    right: -10px;
	    top: 9px;
	  }
	  .controls {
	    height: 80px;
	    width: 25px;
	    background: #DDDDDD;
	    border: 4px inset rgba(123, 123, 123, 0.867);
	    border-radius: 5px;
	    bottom: 10px;
	    left: 25px;
	    margin: 0 auto;
	    position: absolute;
	    display: flex;
	    align-items: center;
	  }
	  .speed {
	    height: 70px;
	    width: 5px;
	    background: rgb(91, 91, 91);
	    margin: 0 auto;
	    
	  }
	  .lever {
	    height: 10px;
	    width: 17.5px;
	    background: #212121;
	    border: 2px solid #000;
	    position: absolute;
	    left: 2px;
	    top: 35px;
	  }
	  
	  @keyframes nowPlaying {
	    0% { 
	      transform: rotate(0deg)
	    }
	    100% {
	      transform: rotate(360deg)
	    }
	  }
  </style>
</head>
<body>
  <section class="turntable">
    <div class="plinth">
      <div class="start"></div>
      <div class="strobe"></div>
      <div class="adapter">
        <div class="innerAdapter"></div>
      </div>
      <div class="speedButton">
        <div class="thirtyThree"></div>
        <div class="fortyFour"></div>
      </div>
      <div class="platterContainer">
        <div class="platter">
          <div class="record">
            <div class="grooveLine">
              <div class="grooveInner">
                <div class="innerGroove"></div>
              </div>
            </div>
            <div class="label">
              <div class="labelL"></div>
              <div class="labelR"></div>
            </div>
          </div>
          <div class="spindle"></div>
        </div>
      </div>
      <div class="rightSide">
          <div class="armBase">
            <div class="innerBase"></div>
          </div>
        <div class="arm">
          <div class="counterWeight"></div>
          <div class="armBend"></div>
          <div class="armBendTwo"></div>
          <div class="cartridge">
            <div class="lift"></div>
          </div>
        </div>
        <div class="controls">
          <div class="speed">
            <div class="lever"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</body>
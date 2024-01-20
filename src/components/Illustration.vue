<template>
  <div class="illustration">
    <div class="container">
      <div class="clouds">
        <div class="cloud one"></div>
        <div class="cloud two"></div>
        <div class="cloud three"></div>
      </div>

      <div class="sun"></div>
      <div class="bosh">
        <div class="body">
          <div class="part one"></div>
          <div class="part two"></div>
        </div>
      </div>
      <div class="tree">
        <div class="leaves"></div>
        <div class="root">
          <div class="branch one"></div>
          <div class="branch two"></div>
          <div class="branch three"></div>
        </div>
        <div class="ground"></div>
        <div class="car">
          <div class="body">
            <div class="top">
              <div class="window left"></div>
              <div class="window right"></div>
            </div>
            <div class="main"></div>
            <div class="wheels">
              <div class="left"></div>
              <div class="right"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.illustration,
.illustration *,
.illustration *::before,
.illustration *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.illustration {
  margin: 4em 0;
  width: 100%;
  display: grid;
  place-items: center;
  font-family: Arial, Helvetica, sans-serif;
  background-color: rgb(205, 252, 255);
}

.container {
  position: relative;
}

.clouds {
  position: absolute;
  right: -20px;
  top: 0;
}

.cloud {
  height: 30px;
  width: 100px;
  background-color: rgb(243, 249, 254);
  border-radius: 9999px;
}

.cloud.one {
  margin-left: 70px;
}
.cloud.two {
  margin-left: 40px;
}
.cloud.three {
  margin-left: 10px;
}

.tree {
  position: relative;
}

.tree .leaves {
  height: 120px;
  width: 70px;
  border-radius: 9999px;
  background: linear-gradient(to top, rgb(132, 205, 132), rgb(190, 254, 190));
}

.tree .root {
  height: 85px;
  width: 4px;
  background-color: black;
  position: absolute;
  bottom: -30px;
  right: 50%;
  transform: translateX(50%);
  border-radius: 9999px 0;
}

.branch {
  background-color: black;
  height: 20px;
  width: 3px;
  position: absolute;
  border-radius: 9999px 0;
}
.branch.one {
  top: 17px;
  right: 6px;
  transform: rotate(-30deg);
}
.branch.two {
  top: 15px;
  right: -5px;
  transform: rotate(30deg);
}
.branch.three {
  top: -8px;
  right: 6px;
  transform: rotate(-30deg);
}

.tree .ground {
  width: 200px;
  height: 3px;
  background-color: black;
  position: absolute;
  bottom: -30px;
  right: 50%;
  transform: translateX(50%);
  border-radius: 9999px;
}

.bosh {
  position: absolute;
  bottom: -30px;
  right: -50px;
}

.bosh.body {
  position: relative;
}

.part {
  background: linear-gradient(
    to top,
    rgb(167, 241, 132),
    rgb(167, 241, 132),
    rgb(197, 248, 173)
  );
}

.part.one {
  width: 60px;
  height: 30px;
  border-radius: 9999px;
}
.part.two {
  height: 40px;
  width: 40px;
  border-radius: 9999px;
  position: absolute;
  top: -15px;
  right: 50%;
  transform: translateX(50%);
}
.sun {
  height: 50px;
  width: 50px;
  position: absolute;
  top: -30px;
  right: -60px;
  border-radius: 50%;
  background: radial-gradient(rgb(254, 239, 155), rgb(252, 208, 94));
}

.car {
  position: absolute;
  bottom: -20px;
  left: -65px;
}

.car .body {
  position: relative;
}

.car .top {
  width: 50px;
  height: 20px;
  background: linear-gradient(
    to top,
    rgb(0, 76, 255),
    rgb(0, 76, 255),
    rgb(96, 169, 252)
  );
  border-radius: 9999px 9999px 0 0;
  position: absolute;
  top: -10px;
  right: 50%;
  transform: translateX(50%);
  display: flex;
  gap: 3px;
  justify-content: center;
  align-items: center;
}

.window {
  height: 12px;
  width: 20px;
  background-color: rgb(187, 236, 243);
  -webkit-clip-path: polygon(100% 2%, 31% 2%, 0 100%, 100% 100%);
  clip-path: polygon(100% 2%, 31% 2%, 0 100%, 100% 100%);
}

.window.right {
  -webkit-clip-path: polygon(76% 2%, 0 0, 0 100%, 100% 100%);
  clip-path: polygon(76% 2%, 0 0, 0 100%, 100% 100%);
}
.car .main {
  width: 70px;
  height: 25px;
  background-color: rgb(0, 76, 255);
  border-radius: 9999px 9999px 0 0;
}
.car .wheels {
  position: absolute;
  right: 50%;
  bottom: -10px;
  transform: translateX(50%);
  display: flex;
  gap: 20px;
}

.wheels .left,
.wheels .right {
  height: 20px;
  width: 20px;
  border-radius: 50%;
  background: radial-gradient(rgb(118, 118, 118), black);
}
</style>

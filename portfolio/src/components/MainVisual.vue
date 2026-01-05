<template>
<!-- main-visual -->
<div class="main-visual">
  <div class="main-visual-inner">
    <p class="main-visual-title">{{ name }}</p>
    <p class="main-visual-subtitle">ABOUT ME</p>
  </div>
  <div class="main-visual-area" >
    <ul class="main-visual-circles">
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
    </ul>
  </div >
</div>
<!-- /main-visual -->
</template>

<script>
export default {
  name: 'MainVisual',
  data () {
    return {
      name: 'H.Y'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*--------------------------------
メインビジュアル
---------------------------------*/
.main-visual {
  display: flex;
  width: 100%;
  align-items: center;
  justify-content: center;
  height: 35vh;
  text-align: center;
  overflow-x: hidden;
}
.main-visual-inner {
  width: 100%;
  position: absolute;
  padding: 0 40px;
}
.main-visual-title {
  font-size: 60px;
  font-weight: bold;
  line-height: 1.2;
  margin-bottom: 5px;
  letter-spacing: .1em;
}
.main-visual-subtitle {
  font-size: 20px;
  font-weight: bold;
  line-height: 1;
  margin-bottom: 40px;
  letter-spacing: .08em;
}
.main-visual-area {
  width: 100%;
  height: 35vh;
  background: #fff;
}
.main-visual-circles {
  position: relative;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 35vh;
  margin: 0;
  padding: 0;
  overflow: hidden;
}
.main-visual-circles li {
  position: absolute;
  display: block;
  list-style: none;
  width: 20px;
  height: 20px;
  background: rgba(214,233,202,.5);
  animation: animate 25s linear infinite;
  bottom: -150px;
}
.main-visual-circles li:nth-child(1) {
  left: 25%;
  width: 80px;
  height: 80px;
  animation-delay: 0s;
}
.main-visual-circles li:nth-child(2) {
  left: 10%;
  width: 80px;
  height: 80px;
  animation-delay: 2s;
  animation-duration: 12s;
}
.main-visual-circles li:nth-child(3) {
  left: 70%;
  width: 20px;
  height: 20px;
  animation-delay: 4s;
}
.main-visual-circles li:nth-child(4) {
  left: 40%;
  width: 60px;
  height: 60px;
  animation-delay: 0s;
  animation-duration: 18s;
}
.main-visual-circles li:nth-child(5) {
  left: 65%;
  width: 20px;
  height: 20px;
  animation-delay: 0s;
}
.main-visual-circles li:nth-child(6) {
  left: 75%;
  width: 110px;
  height: 110px;
  animation-delay: 3s;
}
.main-visual-circles li:nth-child(7) {
  left: 35%;
  width: 150px;
  height: 150px;
  animation-delay: 7s;
}
.main-visual-circles li:nth-child(8) {
  left: 50%;
  width: 25px;
  height: 25px;
  animation-delay: 15s;
  animation-duration: 45s;
}
.main-visual-circles li:nth-child(9) {
  left: 20%;
  width: 15px;
  height: 15px;
  animation-delay: 2s;
  animation-duration: 35s;
}
.main-visual-circles li:nth-child(10) {
  left: 85%;
  width: 150px;
  height: 150px;
  animation-delay: 0s;
  animation-duration: 11s;
}
@keyframes animate {
  0% {
    transform: translateY(0) rotate(0deg);
    opacity: 1;
    border-radius: 0;
  }
  100% {
    transform: translateY(-1000px) rotate(720deg);
    opacity: 0;
    border-radius: 50%;
  }
}
/*media Queries 767
---------------------------------------*/
@media screen and (max-width: 767px) {
  /*  メインビジュアル */
  .main-visual-inner {
    padding: 0 20px;
  }
  .main-visual-title {
    font-size: 30px;
  }
  .main-visual-subtitle {
    font-size: 16px;
    margin-bottom: 20px;
  }
}
</style>

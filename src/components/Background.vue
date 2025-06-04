<template>
  <div class="background">
    <div id="stars"></div>
    <div id="stars2"></div>
    <div id="stars3"></div>
  </div>
</template>

<style scoped>
.background {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: radial-gradient(ellipse at bottom, #1B2735 0%, #090A0F 100%);
  z-index: 0;
  overflow: hidden;
}

/* Pequenas estrelas, muitas */
#stars {
  position: absolute;
  width: 1px;
  height: 1px;
  background: transparent;
  box-shadow:
    50px 200px #FFF, 120px 80px #FFF, 150px 100px #FFF, 300px 700px #FFF,
    350px 600px #FFF, 420px 900px #FFF, 500px 800px #FFF, 620px 300px #FFF,
    710px 500px #FFF, 800px 200px #FFF, 900px 400px #FFF, 1000px 350px #FFF,
    1100px 1000px #FFF, 1150px 1100px #FFF, 1200px 600px #FFF, 1300px 200px #FFF,
    1400px 850px #FFF, 1500px 950px #FFF, 1600px 1200px #FFF;
  animation: animStar 50s linear infinite;
}

#stars2 {
  position: absolute;
  width: 2px;
  height: 2px;
  background: transparent;
  box-shadow:
    300px 500px #FFF, 400px 800px #FFF, 600px 900px #FFF, 700px 300px #FFF,
    900px 700px #FFF, 1000px 400px #FFF, 1100px 1100px #FFF, 1300px 600px #FFF;
  animation: animStar 100s linear infinite;
}

#stars3 {
  position: absolute;
  width: 3px;
  height: 3px;
  background: transparent;
  box-shadow:
    800px 700px #FFF, 1100px 1000px #FFF, 1400px 400px #FFF;
  animation: animStar 150s linear infinite;
}

@keyframes animStar {
  from {
    transform: translateY(0);
  }
  to {
    transform: translateY(-2000px);
  }
}
</style>

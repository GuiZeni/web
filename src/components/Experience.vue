<template>
  <div class="container">
    <div class="box">
      <img src="../assets/Img/img 3.png" class="app" />
      <div class="text-content">
        <div class="title">
          <h1>Experimente os recursos QR <br> mais avançados feitos sob medida <br> para suas necessidades.</h1>
        </div>
        <div class="pa">
          <p class="paragraph">
           Crie seus eventos e compartilhe no nosso app para que <br> seus leads possam comprar ingressos e participar com facilidade.
          </p>
        </div>   
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;500;700&display=swap');

.container {
  background-color: rgb(0, 0, 0);
  display: flex;
  justify-content: center;
  align-items: center;
}

.box {
  width: 150vh;
  height: 70vh;
  border-radius: 40px;
  position: relative; 
}

.app
{
  height: 400px;
  position: absolute;
  padding-left: 800px;
  padding-top: 30px;
}


@keyframes floatUpDown {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-15px);
  }
}

.text-content {
  text-align: start;
}

.title {
  color: aliceblue;
  font-family: 'Roboto', sans-serif;
  padding-top: 130px;
  font-size: 20px;
}

.pa {
  padding-top: 75px;
  padding-left: 0px;
}

.paragraph {
  color: aliceblue;
  font-size: 25px;
  padding-bottom: 10px;
  
  font-family: 'Roboto', sans-serif;
}
</style>

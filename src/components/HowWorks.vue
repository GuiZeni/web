<template>
  <div class="container">
    <div class="box">
      <img src="../assets/Img/app.png" class="app" />
      <img src="../assets/Img/app.png" class="app2" />
      <img src="../assets/Img/app.png" class="app3" />
      <div class="text-content">
        <div class="title">
          <h1>Como funciona o App</h1>
        </div>
        <div class="pa">
          <p class="paragraph">
            Com o QR Connect, tudo começa de forma <br /> simples: baixe o  
            aplicativo, faça seu cadastro <br /> e crie sua conta. personalizada de
            acordo <br /> com suas necessidades. Para participar de um evento, 
            será gerado um  QR Ticket exclusivo.<br /> Basta apresentá-lo na         
            entrada do evento e,<br /> após a validação, seu ingresso será
            <br /> confirmado — pronto! É só aproveitar a festa. 
          </p>
        </div>   
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;500;700&display=swap');

.container {
  background-color: rgb(20, 20, 20);
  display: flex;
  justify-content: center;
  align-items: center;
}

.box {
  background-color: #1f1f1f;
  width: 150vh;
  height: 70vh;
  border-radius: 40px;
  position: relative; 
}

.app,
.app2,
.app3 {
  height: 600px;
  position: absolute;
  animation: floatUpDown 4s ease-in-out infinite;
}

.app {
  left: 10%;
  top: 8%;
  animation-delay: 0s;
}

.app2 {
  left: -5%;
  top: 13%;
  animation-delay: 1.3s;
}

.app3 {
  left: 25%;
  top: 13%;
  animation-delay: 2.6s;
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
  padding-top: 90px;
  padding-left: 875px;
  font-size: 20px;
}

.pa {
  padding-top: 75px;
  padding-left: 840px;
}

.paragraph {
  color: aliceblue;
  font-size: 25px;
  padding-bottom: 10px;
  font-family: 'Roboto', sans-serif;
}



</style>

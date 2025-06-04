<template>
  <div class="container">
    <div class="box">
      <div class="pa">
        <p class="paragraph">
          INSTALE JÁ
        </p>
      </div>   
      <div class="text-content">
        <div class="title">
          <h1>Experimente o QR Connect e impulsione <br> suas vendas com praticidade e inovação.</h1>
        </div>

        <div class="button-position">
            <button class="download" type="button" aria-label="Instale o aplicativo QR Connect">
          <img src="../assets/Img/DownloadIcon.png" alt="Ícone de download" class="download-icon" />
          <div class="download-info">
            <p>Instale o app aqui</p>
            <h2>QR Connect</h2>
          </div>
        </button>
        </div>
        
      </div>   
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;500;700&display=swap');

.container {
  background-color: rgb(26, 25, 25);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh; 
}

.box {
  background: linear-gradient(90deg, #12106e 0%, #11101e 100%);
  width: 150vh;
  height: 70vh;
  border-radius: 40px;
  position: relative; 
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding: 40px 20px;
  box-sizing: border-box;
}

.paragraph {
  color: aliceblue;
  font-size: 25px;
  font-family: 'Roboto', sans-serif;
  margin: 0;
  padding-top: 90px;
  font-weight: 700;
  letter-spacing: 1.5px;
}

.title {
padding-top: 30px;
  color: aliceblue;
  font-family: 'Roboto', sans-serif;
  font-size: 25px;
  margin-bottom: 40px;
  line-height: 1.3;
}
.button-position{
    padding-top: 30px;
}
.download {
  display: flex;
  align-items: center;
  gap: 1rem;
  border: 2px solid #ffffff;
  border-radius: 8px;
  padding: 1rem 2rem;
  background-color: transparent;
  cursor: pointer;
  transition: border-color 0.3s ease, background-color 0.3s ease;
  max-width: 350px;
  margin: 0 auto;
}

.download:hover,
.download:focus {
  border-color: #007bff;
  background-color: #132335;
  outline: none;
}

.download-icon {
  width: 50px;
  height: 50px;
}

.download-info p {
  margin: 0;
  font-size: 14px;
  color: #ffffff;
}

.download-info h2 {
  margin: 0;
  font-size: 20px;
  color: #ffffff;
}

@media (max-width: 768px) {
  .box {
    width: 90vw;
    height: auto;
    padding: 30px 15px;
  }

  .title {
    font-size: 20px;
    margin-bottom: 30px;
  }

  .paragraph {
    font-size: 20px;
  }

  .download {
    flex-direction: column;
    padding: 1rem;
    text-align: center;
    max-width: 100%;
  }

  .download-icon {
    width: 40px;
    height: 40px;
  }
}
</style>

<template>
  <div class="overlay-content">
    <span class="gradient-text">
      Deixe o QR te levar. <br />
      Conecte-se aos melhores eventos <br />
      com o QR Connect.
    </span>
    <span class="gradient-subtext">
      Crie, divulgue e gerencie seus eventos em minutos.
    </span>

    <button class="download" type="button" aria-label="Instale o aplicativo QR Connect">
      <img :src="DownloadIcon" alt="Ícone de download" class="download-icon" />
      <div class="download-info">
        <p>Instale o app aqui</p>
        <h2>QR Connect</h2>
      </div>
    </button>
  </div>
</template>

<script setup>
import DownloadIcon from '../assets/Img/DownloadIcon.png';
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;700&display=swap');

.overlay-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  padding: 2rem;
  color: white;
  text-align: center;
  font-family: 'Manrope', sans-serif;
  gap: 3rem;
  z-index: 1;
  position: relative;
}

.gradient-text {
  font-size: 2.5rem;
  font-weight: 500;
  background: -webkit-linear-gradient(white, #38495a);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  line-height: 1.4;
}

.gradient-subtext {
  font-size: 1.2rem;
  color: white;
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
  .overlay-content {
    font-size: 1.5rem;
  }

  .download {
    flex-direction: column;
    padding: 1rem;
    text-align: center;
  }

  .download-icon {
    width: 40px;
    height: 40px;
  }
}
</style>

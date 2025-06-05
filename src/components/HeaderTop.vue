<script setup lang="ts">
// Nenhum script necessário por enquanto
</script>

<template>
  <header>
    <nav aria-label="Main Navigation" class="nav-container">
      <div class="left-logos">
        <img src="../assets/Img/Logo.png" alt="Logo" class="Logo" />
        <img src="../assets/Img/QrConnectTxt.png" alt="QR Connect Text" class="ImgTxt" />
      </div>
      <ul class="nav-links">
        <li><a href="#inicio" class="home">Início</a></li>
        <li><a href="#como-funciona" class="how-work">Como Funciona</a></li>
        <li><a href="#contact" class="contact-us">Contate-nos</a></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

header {
  font-family: 'Roboto', sans-serif;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #00000000;
  padding: 20px 0;
  z-index: 1000;
  box-shadow: 0 4px 12px rgba(255, 255, 255, 0.2);
}

.nav-container {
  position: relative;
  width: 100%;
  height: 60px;
}

.left-logos {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  display: flex;
  align-items: flex-end;
  gap: 4px;
  padding-left: 1rem;
}

.nav-links {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  gap: 2rem;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-links li {
  text-align: center;
}

a {
  text-decoration: none;
  color: #bebebe;
  font-size: 18px;
  font-weight: 500;
  transition: color 0.3s ease;
}

a:hover {
  color: #ffffff;
}

.ImgTxt {
  height: 220px;
  position: absolute;
  left: 30%;
  top: -55%;
}

.Logo {
  height: 110px;
}

/* Responsividade */

@media (max-width: 1440px) {
  .ImgTxt {
    height: 180px;
    top: -47%;
    left: 35%;
  }
  .Logo {
    height: 100px;
  }
}

@media (max-width: 1024px) {
  .ImgTxt {
    height: 150px;
    top: -45%;
    left: 40%;
  }
  .Logo {
    height: 85px;
  }
  .nav-links {
    gap: 1.5rem;
  }
  a {
    font-size: 16px;
  }
}

@media (max-width: 768px) {
  .ImgTxt {
    height: 120px;
    top: -40%;
    left: 40%;
  }
  .Logo {
    height: 70px;
  }
  .nav-links {
    gap: 1.2rem;
  }
  a {
    font-size: 15px;
  }
}

@media (max-width: 600px) {
  .ImgTxt {
    height: 100px;
    top: -30%;
    left: 20%;
  }
  .Logo {
    height: 60px;
  }
  .nav-links {
    gap: 1rem;
  }
  a {
    font-size: 14px;
  }
}

@media (max-width: 480px) {
  .ImgTxt {
    height: 90px;
    top: -25%;
    left: 18%;
  }
  .Logo {
    height: 50px;
  }
  .nav-links {
    flex-direction: column;
    align-items: center;
    top: 120%;
    left: 50%;
    transform: translateX(-50%);
    gap: 0.7rem;
  }
  a {
    font-size: 13px;
  }
}

@media (max-width: 360px) {
  .ImgTxt {
    height: 70px;
    top: -20%;
    left: 16%;
  }
  .Logo {
    height: 45px;
  }
  a {
    font-size: 12px;
  }
}
</style>

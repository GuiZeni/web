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
        <li><a href="#contato" class="contact-us">Contate-nos</a></li>
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

</style>

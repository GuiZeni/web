<script setup lang="ts">
// Nenhuma lógica necessária por enquanto
</script>

<template>
  <div class="container">
    <div class="content-wrapper">
      <div class="text-content">
        <h1>Contate-nos</h1>
        <p>Tem alguma dúvida? Envie-nos uma mensagem</p>
      </div>

      <div class="box">
 
        <div class="info-box">
          <div class="infos">
            <h1>Informações de Contato</h1>
            <p>Envie uma mensagem para retornarmos o contato</p>

            <div class="info-item">
              <img src="../assets/Img/phone.png" alt="Telefone" />
              <span>+55 45 99843-1882</span>
            </div>

            <div class="info-item">
              <img src="../assets/Img/Email.png" alt="Email" />
              <span>QrConnect@gmail.com</span>
            </div>

            <div class="info-item">
              <img src="../assets/Img/Local.png" alt="Localização" />
              <span>Cascavel, Paraná</span>
            </div>
          </div>
        </div>

        <div class="form-box">
          <div class="row">
            <input type="text" placeholder="Nome" class="input" />
            <input type="text" placeholder="Sobrenome" class="input" />
          </div>

          <div class="row single">
            <input type="email" placeholder="Email" class="input" />
          </div>

          <div class="row single">
            <input type="tel" placeholder="Numero de Telefone" class="input" />
          </div>

          <div class="row single">
            <label class="subject-label">Escreva sua mensagem</label>
           
          </div>

          <div class="row single">
            <textarea placeholder="Digite aqui..." class="textarea"></textarea>
          </div>

          <div class="row single">
            <button class="submit-btn">Send Message</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;400;500;700&display=swap');

* {
  box-sizing: border-box;
}

body, html {
  margin: 0;
  padding: 0;
  background-color: #d4d4d4;
  font-family: 'Roboto', sans-serif;
}

.container {
  background-color: #1b1b1b;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 60px 20px;
  color: #fff;
  font-family: 'Roboto', sans-serif;
}

.content-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.text-content h1 {
  font-size: 36px;
  padding-left: 10px;
  margin-bottom: 10px;
  color: white;
}

.text-content p {
  font-size: 18px;
  color: #ccc;
  margin-bottom: 30px;
}

.box {
  background-color: #000000;
  width: 100%;
  max-width: 1200px;
  border-radius: 12px;
  display: flex;
  flex-wrap: wrap;
  padding: 30px;
  gap: 20px;
  justify-content: center;
}

.info-box {
  background-color: #2a2a2a;
  border-radius: 10px;
  padding: 20px;
  color: #fff;
  flex: 1 1 300px;
  max-width: 400px;
}

.infos h1 {
  margin-bottom: 10px;
  font-size: 20px;
}

.infos p {
  margin-bottom: 20px;
}

.info-item {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
  gap: 10px;
}

.info-item img {
  width: 30px;
  height: 30px;
}

/* Formulário */
.form-box {
  flex: 2 1 400px;
  display: flex;
  flex-direction: column;
  gap: 20px;
  padding: 20px;
  background-color: #2f2f2f;
  border-radius: 10px;
}

.row {
  display: flex;
  gap: 15px;
}

.row.single {
  flex-direction: column;
  gap: 10px;
}

.input, .textarea {
  flex: 1;
  padding: 12px;
  font-size: 16px;
  border: none;
  border-bottom: 1px solid #555;
  background-color: transparent;
  color: white;
}

.input::placeholder,
.textarea::placeholder {
  color: #aaa;
  font-weight: 300;
}

.textarea {
  resize: vertical;
  min-height: 100px;
}

.submit-btn {
  padding: 14px 24px;
  font-size: 16px;
  background-color: #111;
  color: white;
  border: 1px solid #444;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.submit-btn:hover {
  background-color: #333;
}

.subject-label {
  font-size: 14px;
  color: #ccc;
  margin-bottom: 5px;
}

.subject-options {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}

.subject-options label {
  color: #ccc;
  font-size: 14px;
  display: flex;
  align-items: center;
  gap: 5px;
}

.subject-options input[type="radio"] {
  accent-color: white;
}

/* Responsivo */
@media (max-width: 768px) {
  .box {
    flex-direction: column;
    align-items: center;
  }

  .row {
    flex-direction: column;
  }
}
</style>

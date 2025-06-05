<template>
  <div class="container">
    <div class="content-wrapper">
      <div class="textMain">
        <h1>Contate-nos</h1>
        <p>Envie-nos um email para podermos conversar</p>
      </div>

      <div class="form-wrapper">
        <div class="left-panel">
          <div class="circle circle-1"></div>
          <div class="circle circle-2"></div>
        </div>

        <div class="form-container">
          <form class="form" @submit.prevent="sendEmail" ref="formRef">
            <div class="row double">
              <input type="text" name="first_name" placeholder="Nome" required />
              <input type="text" name="last_name" placeholder="Sobrenome" />
            </div>

            <div class="row single">
              <input type="email" name="email" placeholder="Email" required />
            </div>

            <div class="row single">
              <input type="tel" name="phone" placeholder="Telefone"/>
            </div>

            <div class="row single">
            </div>

            <div class="row single">
              <label class="label">Message</label>
              <textarea name="message" placeholder="Escreva aqui.." required></textarea>
            </div>

            <div class="row single">
              <button type="submit" class="submit-btn">Envie sua mensagem</button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import emailjs from '@emailjs/browser'

const formRef = ref(null)

const sendEmail = () => {
  emailjs.sendForm(
    'service_vuxqduc',     
    'template_37q2pkk',    
    formRef.value,
    'LcK5_jMWJHgYvL7uM'     
  ).then(
    () => {
      alert('Mensagem enviada com sucesso!')
      formRef.value.reset()
    },
    (error) => {
      alert('Erro ao enviar. Tente novamente.')
      console.error(error.text)
    }
  )
}
</script>

<style scoped>
.container {
  background: #1a1a1a;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  padding: 40px;
  font-family: 'Roboto', sans-serif;
}

.content-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  padding-top: 170px;
  max-width: 1200px;
}

.textMain {
  text-align: center;
  color: white;
  margin-bottom: 40px;
}

.textMain h1 {
  font-size: 36px;
  margin-left: 30px;
  margin-bottom: 10px;
}

.textMain p {
  font-size: 18px;
  margin-left: 20px;
  color: #cccccc;
}

.form-wrapper {
  display: flex;
  width: 100%;
  max-width: 1200px;
  height: auto;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 0 15px rgba(0,0,0,0.1);
}

.left-panel {
  flex: 1;
  background-color: #000;
  position: relative;
  min-height: 500px;
}

.circle {
  position: absolute;
  background-color: rgba(255, 255, 255, 0.05);
  border-radius: 50%;
}

.circle-1 {
  width: 120px;
  height: 120px;
  bottom: 40px;
  left: 30px;
}

.circle-2 {
  width: 200px;
  height: 200px;
  bottom: 0;
  left: 80px;
}

.form-container {
  flex: 2;
  background: #070707;
  padding: 40px;
}

.form {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.row {
  display: flex;
  gap: 20px;
  justify-content: center;
  
}

.row.double input {
  flex: 1;
}

.row.single {
  flex-direction: column;
  
}

input,
textarea {
  width: 100%;
  padding: 12px;
  border: none;
  border-bottom: 1px solid #ccc;
  background-color: transparent;
  color: #cccccca9; 
  font-size: 16px;
}

input::placeholder,
textarea::placeholder {
  color: #cccccca9; 
}

textarea {
  min-height: 100px;
  resize: vertical;
  font-family: 'Roboto', sans-serif;

}

.label {
  font-weight: bold;
  margin-bottom: 5px;
  font-size: 14px;
}

.submit-btn {
  background: #000;
  color: white;
  padding: 14px 24px;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  font-size: 16px;
  align-self: flex-start;
}

.submit-btn:hover {
  background-color: #333;
}

@media (max-width: 768px) {
  .form-wrapper {
    flex-direction: column;
  }

  .left-panel {
    height: 200px;
  }
}
</style>

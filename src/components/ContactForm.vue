<script setup lang="ts">
import { ref } from 'vue'
const WEB3FORMS_ACCESS_KEY = 'YOUR_ACCESS_KEY_HERE'
const name = ref('')
const email = ref('')
const message = ref('')

const submitForm = async () => {
  const response = await fetch('https://api.web3forms.com/submit', {
    method: 'POST',
    headers: {
      'Content-Type': 'application/json',
      Accept: 'application/json',
    },
    body: JSON.stringify({
      access_key: WEB3FORMS_ACCESS_KEY,
      name: name.value,
      email: email.value,
      message: message.value,
    }),
  })
  const result = await response.json()
  if (result.success) {
    console.log(result)
  }
}
</script>

<template>
  <form @submit.prevent="submitForm" class="contact-form">
    <input type="text" name="name" v-model="name" placeholder="Ваше имя" class="form-input" />
    <input type="email" name="email" v-model="email" placeholder="Ваш email" class="form-input" />
    <textarea
      name="message"
      v-model="message"
      placeholder="Ваше сообщение"
      class="form-textarea"
    ></textarea>
    <button type="submit" class="form-button">Отправить сообщение</button>
  </form>
</template>

<style scoped>
.contact-form {
  display: flex;
  flex-direction: column;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  background-color: #f9f9f9;
}

.form-input,
.form-textarea {
  margin-bottom: 15px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  font-size: 16px;
}

.form-input:focus,
.form-textarea:focus {
  border-color: #007bff;
  outline: none;
}

.form-button {
  padding: 10px 15px;
  border: none;
  border-radius: 4px;
  background-color: #007bff;
  color: white;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.form-button:hover {
  background-color: #0056b3;
}
</style>

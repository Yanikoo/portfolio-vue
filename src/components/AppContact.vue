<template>
  <div class="container">
    <h2 class="container__title">Связаться со мной</h2>
    <p class="container__text">Есть вопросы? Напишите мне и я обязательно отвечу!</p>

    <div class="container__block">
      <div class="container__card">
        <div class="container__card-icon"></div>
        <img src="../assets/images/icons/phone-call.svg" alt="phone-call" />
      </div>

      <div class="container__form">
        <ContactForm />
      </div>
    </div>
  </div>
</template>

<script>
import ContactForm from './ContactForm.vue'
export default {
  components: { ContactForm },
}
</script>

<style scoped lang="scss">
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #030712;
  width: 100%;
  height: 100vh;

  &__title {
    font-size: 20px;
    padding: 0 10px;
    font-weight: lowercase;
    color: #000000;
    background-color: #d1d5db;
    border-radius: 12px;
    margin-bottom: 16px;
    margin-top: 96px;
  }
  &__text {
    font-size: 20px;
    font-weight: lowercase;
    color: #ffffff;
    margin-bottom: 48px;
  }
  &__block {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 1440px;
    height: 560px;
  }
  &__card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
  }
}
</style>

<template>
  <div class="container" id="portfolio">
    <h2 class="container__title">Портфолио</h2>
    <p class="container__text">Портфолио, на котором вы можете увидеть мои проекты.</p>
    <div class="container__block">
      <PortolioOne />
    </div>
  </div>
</template>

<script>
import PortolioOne from './parts/PortolioOne.vue'

export default {
  components: {
    PortolioOne,
  },
}
</script>

<style scoped lang="scss">
.container {
  width: 100%;
  height: 560px;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 96px;
  &__title {
    font-size: 20px;
    padding: 0 10px;
    font-weight: lowercase;
    color: #4b5563;
    background-color: #d1d5db;
    border-radius: 12px;
    margin-bottom: 16px;
  }
  &__text {
    font-size: 20px;
    font-weight: lowercase;
    color: #4b5563;
    margin-bottom: 48px;
  }
  &__block {
    width: 1152px;
    height: 480px;
    border-radius: 15px;
    box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.25);
    background-color: #ffffff;
  }
}
</style>

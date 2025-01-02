<template>
  <div class="container">
    <nav class="navbar">
      <img src="../assets/img/vuelog.png" alt="" width="90" height="40" />
      <ul class="navbar__list">
        <li><a href="#stack">Технологии</a></li>
        <li><a href="#portfolio">Портфолио</a></li>
        <li><a href="#section3">Об мне</a></li>
        <li><a href="#section4">Контакты</a></li>
      </ul>
      <ThemeToggle @toggle-theme="toggleTheme" />
    </nav>
  </div>
  <HeadrMain />
</template>

<script>
import ThemeToggle from './ThemeToggle.vue'
import HeadrMain from './HeadrMain.vue'
export default {
  components: { ThemeToggle, HeadrMain },
  data() {
    return {
      isDarkMode: false, // Начальное состояние (светлый режим)
    }
  },
  methods: {
    toggleTheme() {
      this.isDarkMode = !this.isDarkMode // Переключаем состояние темы
      document.body.classList.toggle('dark-mode', this.isDarkMode) // Добавляем классы для смены темы
    },
  },
}
</script>

<style scoped lang="scss">
.container {
  width: 100%;
  max-width: 1440px;
  margin: 0 auto;
  padding: 0 20px;
  box-sizing: border-box;
  margin-bottom: 90px;
}
.navbar {
  height: 68px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: fixed; // Фиксированное положение
  background: #e5e7eb;
  margin: 0;
  top: 0;
  left: 0;
  right: 0;
  padding: 20px 0;
  z-index: 1000;
  transition: background-color 0.3s ease;

  &__list {
    display: flex;
    gap: 20px;
  }
}
</style>

<template>
  <div class="container">
    <nav :class="['navbar', { 'dark-mode': isDarkMode }]">
      <img src="../assets/img/vuelog.png" alt="" width="90" height="40" />
      <ul class="navbar__list">
        <li><a href="#">Технологии</a></li>
        <li><a href="#">Портфолио</a></li>
        <li><a href="#">Об мне</a></li>
        <li><a href="#">Контакты</a></li>
      </ul>
      <ThemeToggle @toggle-theme="toggleTheme" />
      <!-- Используйте ваш новый компонент -->
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
.dark-mode {
  background-color: #1a1a1a;
  color: #ffffff;
}

.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  box-sizing: border-box;
  margin-bottom: 90px;
}
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;

  &__list {
    display: flex;
    gap: 20px;
  }
}
</style>

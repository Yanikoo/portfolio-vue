<template>
  <div class="container" id="portfolio">
    <h2 class="container__title">Портфолио</h2>
    <p class="container__text">Портфолио, на котором вы можете увидеть мои проекты.</p>
    <div class="container__block">
      <PortfolioTree />
    </div>
    <div class="container__block">
      <PortfolioTwo />
    </div>
    <div class="container__block">
      <PortfolioOne />
    </div>
    <div class="container__block" v-for="project in displayedProjects" :key="project.id">
      <PortfolioOne :project="project" />
    </div>
    <button class="container__button" v-if="!isExpanded" @click="expandPortfolio">
      Еще проекты
    </button>
    <button class="container__button-close" v-if="isExpanded" @click="collapsePortfolio">
      Закрыть
    </button>
  </div>
</template>

<script>
import PortfolioOne from './parts/PortfolioOne.vue'
import PortfolioTwo from './parts/PortfolioTwo.vue'
import PortfolioTree from './parts/PortfolioTree.vue'

export default {
  data() {
    return {
      projects: [
        { id: 1, title: 'Проект 1', description: 'Описание проекта 1' },
        { id: 2, title: 'Проект 2', description: 'Описание проекта 2' },
      ],
      isExpanded: false,
    }
  },
  computed: {
    displayedProjects() {
      return this.isExpanded ? this.projects : []
    },
  },
  methods: {
    expandPortfolio() {
      this.isExpanded = true
    },
    collapsePortfolio() {
      this.isExpanded = false
    },
  },
  components: {
    PortfolioOne,
    PortfolioTwo,
    PortfolioTree,
  },
}
</script>

<style scoped lang="scss">
@import '@/assets/media.css';
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #1f2937;
  margin-top: -40px;
  &__title {
    font-size: 20px;
    padding: 0 10px;
    font-weight: lowercase;
    color: #4b5563;
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
    border-radius: 15px;
    box-shadow: 0px 4px 16px rgba(250, 249, 249, 0.856);
    background-color: #ffffff;
    margin: 24px;
  }
  &__button {
    width: 150px;
    height: 30px;
    font-size: 20px;
    font-weight: lowercase;
    color: #ffffff;
    background-color: #10b981;
    border-radius: 12px;
    margin-bottom: 16px;
    margin-top: 96px;
  }
  &__button:hover {
    background-color: #0d6d57;
    color: #d1d5db;
    cursor: pointer;
  }
  &__button-close {
    width: 150px;
    height: 30px;
    font-size: 20px;
    font-weight: lowercase;
    color: #ffffff;
    background-color: #e90e0e;
    border-radius: 12px;
    margin-bottom: 16px;
    margin-top: 96px;
  }
  &__button-close:hover {
    background-color: #290303;
    color: #d1d5db;
    cursor: pointer;
  }
}
</style>

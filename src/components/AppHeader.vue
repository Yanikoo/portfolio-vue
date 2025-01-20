<template>
  <div class="container">
    <nav class="navbar">
      <p class="navbar__title">< Vue Portfolio /></p>
      <ul :class="['navbar__list', { 'navbar__list-active': isActive }]">
        <li class="navbar__list-item"><a href="#stack">Технологии</a></li>
        <li class="navbar__list-item"><a href="#portfolio">Портфолио</a></li>
        <li class="navbar__list-item"><a href="#section3">Об мне</a></li>
        <li class="navbar__list-item"><a href="#section4">Контакты</a></li>
      </ul>
      <button @click="toggleMenu" class="navbar__btn" :class="{ active: isActive }">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </nav>
    <HeadrMain />
  </div>
</template>

<script>
import HeadrMain from './HeadrMain.vue'
export default {
  data() {
    return {
      isActive: false,
    }
  },
  methods: {
    toggleMenu() {
      this.isActive = !this.isActive
      // console.log(this.isActive)
    },
  },
  components: { HeadrMain },
}
</script>

<style scoped lang="scss">
.container {
  max-width: 100%;
  margin: 0 auto;
  box-sizing: border-box;
  background-color: #d1d5db;
}
.navbar {
  height: 68px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: fixed;
  background: #e5e7eb;
  margin: 0 auto;
  top: 0;
  left: 0;
  right: 0;
  padding: 0 20px;
  z-index: 1000;
  transition: background-color 0.3s ease;

  &__list {
    display: flex;
    gap: 20px;
    font-size: 20px;
    font-weight: bold;
  }
  &__list-item:hover {
    color: #0c0fb9;
  }

  &__title {
    font-size: 30px;
    font-weight: bold;
    color: #048119;
  }
  &__btn {
    width: 30px;
    height: 25px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 0;
    background-color: transparent;
    border: none;
    cursor: pointer;
    display: none;
  }
  span {
    height: 2px;
    width: 100%;
    background-color: #000000;
  }
}

@media screen and (max-width: 940px) {
  .navbar {
    display: flex;
    justify-content: space-between;

    &__btn {
      display: flex;
    }
    &__btn,
    &__title {
      position: relative;
      z-index: 10;
    }
    &__title {
      font-size: 25px;
      font-weight: bold;
      // color: #1c776b;
    }
    &__list {
      position: fixed;
      z-index: 5;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      background-color: #151515;
      top: 0;
      left: 0;
      right: 0;
      height: auto;
      padding-top: 100px;
      padding-bottom: 100px;
      color: #d1d5db;
      transform: translateY(-100%);
      transition: transform 0.3s ease;
    }
  }
  .navbar__list-active {
    transform: translateY(0);
    display: flex;
  }
}
.navbar__btn.active span {
  background-color: #fff;
}
</style>

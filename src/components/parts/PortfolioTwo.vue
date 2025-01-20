<template>
  <div class="main">
    <div class="main__block">
      <h3 class="main__title">Leasing From D&M</h3>
      <p class="main__text">
        Много страничный сайта с форомой отправки контактов и картинками на класическо HTML, CSS,
        JS. С добовлением слайдом Swiper.js и пагинацией. Так же сдела адоптив под все устройства.
        Верста написана с методологией БЭМ.
      </p>
      <div class="main__element">
        <p>HTML</p>
        <p>CSS</p>
        <p>JS</p>
        <p>SVG</p>
        <p>GitHub</p>
        <p>BEM</p>
        <p>Figma</p>
      </div>
      <a href="https://poject-shop.vercel.app/new-cars.html" target="_blank">
        <svg
          width="36"
          height="36"
          viewBox="0 0 36 36"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M24 19V25C24 25.5304 23.7893 26.0391 23.4142 26.4142C23.0391 26.7893 22.5304 27 22 27H11C10.4696 27 9.96086 26.7893 9.58579 26.4142C9.21071 26.0391 9 25.5304 9 25V14C9 13.4696 9.21071 12.9609 9.58579 12.5858C9.96086 12.2107 10.4696 12 11 12H17"
            stroke="#4B5563"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M21 9H27V15"
            stroke="#4B5563"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M16 20L27 9"
            stroke="#4B5563"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>
      </a>
    </div>
    <div class="main__img-block">
      <a href="https://poject-shop.vercel.app/new-cars.html" target="_blank">
        <img class="main__img" src="@\assets\img\shop.jpg" alt="демонстрация работы" />
      </a>
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style lang="scss">
.main {
  display: flex;
  justify-content: space-between;
  max-width: 1152px;
  // height: 480px;
  // border-radius: 12px;

  &__img-block {
    // width: 575px;
    // height: 480px;
    background-color: #e5e7eb;
    border-radius: 12px;
  }
  &__img {
    max-width: 480px;
    // height: 380px;
    display: block;
    align-items: center;
    // border-radius: 12px;
    // margin: 48px;
    transition: transform 0.5s ease;
  }
  &__img:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
  }
  &__block {
    max-width: 575px;
    // height: 480px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: 25px;
  }
  &__title {
    font-size: 26px;
    font-weight: bold;
    color: #4b5563;
    margin-bottom: 16px;
  }
  &__text {
    font-size: 20px;
    font-weight: lowercase;
    color: #4b5563;
  }
  &__element {
    display: flex;
    flex-wrap: wrap;
    font-size: 20px;
    max-width: 480px;
    height: auto;
    gap: 16px;
    font-weight: lowercase;
    color: #4b5563;
    margin-top: 32px;
    margin-bottom: 20px;
  }
  &__element p {
    padding: 10px 12px;
    font-weight: lowercase;
    color: #4b5563;
    background-color: #d1d5db;
    border-radius: 19px;
    box-sizing: border-box;
    text-align: center;
  }
}
</style>

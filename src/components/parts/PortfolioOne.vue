<template>
  <div class="main">
    <div class="main__img-block">
      <a href="https://project-get-wach.vercel.app/#" target="_blank">
        <img class="main__img" src="@\assets\img\getwatch.jpg" alt="демонстрация работы" />
      </a>
    </div>
    <div class="main__block">
      <h3 class="main__title">GetWatch</h3>
      <p class="main__text">
        Простой одностраничный лэндинг с картинками, кнопками и текстом. Верста написана с
        методологией БЭМ. С переиспользуемой структурой и стилями.
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
      <a href="https://project-get-wach.vercel.app/#" target="_blank">
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
  </div>
</template>

<style lang="scss">
// @import '@/assets/media.css';
// .main {
//   display: flex;
//   flex-wrap: wrap;
//   justify-content: space-between;
//   max-width: 1152px;
//   height: auto;
//   border-radius: 12px;
//   // background-color: #6b7280;

//   &__img-block {
//     flex: 1;
//     min-width: 300px;
//     height: auto;
//   }
//   &__img {
//     width: 100%;
//     height: auto;
//     display: block;
//     align-items: center;
//     border-radius: 12px;
//     margin: 24px;
//     transition: transform 0.5s ease;
//   }
//   &__img:hover {
//     transform: scale(1.05);
//     box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
//   }
//   &__block {
//     flex: 1;
//     display: flex;
//     flex-direction: column;
//     justify-content: center;
//   }
//   &__title,
//   &__text {
//     color: #4b5563;
//     margin-bottom: 16px;
//   }
//   &__title {
//     font-size: 26px;
//   }
//   &__text {
//     font-size: 20px;
//   }
//   &__element {
//     display: flex;
//     flex-wrap: wrap;
//     font-size: 20px;
//     font-weight: lowercase;
//     color: #4b5563;
//   }
//   &__element p {
//     color: #4b5563;
//     background-color: #d1d5db;
//     border-radius: 19px;
//     box-sizing: border-box;
//     text-align: center;
//   }
// }
</style>

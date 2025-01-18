<template>
  <div class="container">
    <div class="container__title">
      <h1 class="container__title-text">
        Привет, я Никита &nbsp;<span class="emoji">&#x1F44B;</span>
      </h1>
      <p class="container__text">
        Я <span class="decorations">фронтенд-разработчик</span>, стремящийся создавать простые и
        интуитивно понятные пользовательские интерфейсы. У меня есть опыт работы с современными
        технологиями, такими как <span class="decorations">Vue.js</span> на языке
        <span class="decorations">JavaScript</span>, что позволяет мне воплощать в жизнь различные
        идеи и концепции. Я увлечен адаптивным дизайном и оптимизацией производительности
        приложений, чтобы обеспечить пользователям лучший опыт. В моем
        <span class="decorations2"><a href="#portfolio">портфолио</a></span> вы найдете проекты,
        которые отражают мой подход к разработке и внимание к деталям.
      </p>

      <div class="container__location">
        <div class="container__location-icon">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M20 10C20 16 12 22 12 22C12 22 4 16 4 10C4 7.87827 4.84285 5.84344 6.34315 4.34315C7.84344 2.84285 9.87827 2 12 2C14.1217 2 16.1566 2.84285 17.6569 4.34315C19.1571 5.84344 20 7.87827 20 10Z"
              stroke="#4B5563"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
            <path
              d="M12 13C13.6569 13 15 11.6569 15 10C15 8.34315 13.6569 7 12 7C10.3431 7 9 8.34315 9 10C9 11.6569 10.3431 13 12 13Z"
              stroke="#4B5563"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
          <div>Москва, Россия</div>
        </div>
        <div class="container__location-icon2">
          <div>
            <svg
              class="pulsating"
              width="8"
              height="8"
              viewBox="0 0 8 8"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect width="8" height="8" rx="4" fill="#10B981" />
            </svg>
          </div>
          <p>Готов рассмотреть интересные предложения по сотрудничеству.</p>
        </div>
        <div class="container__location-nav">
          <a href="https://github.com/Yanikoo" target="_blank">
            <svg
              width="36"
              height="36"
              viewBox="0 0 36 36"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M21 28V24C21.1392 22.7473 20.78 21.4901 20 20.5C23 20.5 26 18.5 26 15C26.08 13.75 25.73 12.52 25 11.5C25.28 10.35 25.28 9.15 25 8C25 8 24 8 22 9.5C19.36 9 16.64 9 14 9.5C12 8 11 8 11 8C10.7 9.15 10.7 10.35 11 11.5C10.2719 12.5159 9.91851 13.7528 10 15C10 18.5 13 20.5 16 20.5C15.61 20.99 15.32 21.55 15.15 22.15C14.98 22.75 14.93 23.38 15 24V28"
                stroke="#4B5563"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M15 24C10.49 26 10 22 8 22"
                stroke="#4B5563"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </a>
          <a href="https://t.me/Kuyzm1ch" target="_blank"
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              x="0px"
              y="0px"
              width="36"
              height="36"
              viewBox="0 0 50 50"
            >
              <path
                d="M25,2c12.703,0,23,10.297,23,23S37.703,48,25,48S2,37.703,2,25S12.297,2,25,2z M32.934,34.375	c0.423-1.298,2.405-14.234,2.65-16.783c0.074-0.772-0.17-1.285-0.648-1.514c-0.578-0.278-1.434-0.139-2.427,0.219	c-1.362,0.491-18.774,7.884-19.78,8.312c-0.954,0.405-1.856,0.847-1.856,1.487c0,0.45,0.267,0.703,1.003,0.966	c0.766,0.273,2.695,0.858,3.834,1.172c1.097,0.303,2.346,0.04,3.046-0.395c0.742-0.461,9.305-6.191,9.92-6.693	c0.614-0.502,1.104,0.141,0.602,0.644c-0.502,0.502-6.38,6.207-7.155,6.997c-0.941,0.959-0.273,1.953,0.358,2.351	c0.721,0.454,5.906,3.932,6.687,4.49c0.781,0.558,1.573,0.811,2.298,0.811C32.191,36.439,32.573,35.484,32.934,34.375z"
              ></path>
            </svg>
          </a>
          <a href="#"><img src="../assets/img/hh-wite.png" alt="#" width="36" height="36" /></a>
        </div>
      </div>
    </div>
    <div class="container__img">
      <img src="../assets/img/myfoto.png" alt="#" width="290" height="360" />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  // width: 100%;
  max-width: 1440px;
  height: 552px;

  &__title {
    width: 600px;
    height: 360px;
    &-text {
      font-size: 40px;
      font-weight: bold;
      color: #4b5563;
    }
  }

  &__location {
    display: flex;
    flex-direction: column;
    align-items: left;
    width: 768px;
    height: 56px;
    margin-top: 30px;

    &-icon {
      display: flex;
      gap: 10px;
      margin-bottom: 8px;
    }
    &-icon2 {
      display: flex;
      gap: 10px;
      margin-left: 7px;
      margin-bottom: 48px;
    }
    &-nav {
      display: flex;
      gap: 10px;
    }
  }

  &__img {
    width: 290px;
    height: 360px;
    // margin-left: 48px;
    box-shadow: 10px 3px 10px rgba(0, 0, 0, 0.3);
  }
  &__img:hover {
    transform: scale(1.05);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.4);
  }
}
.decorations {
  font-weight: bold;
  color: #4b5563;
  text-decoration: underline;
}

.pulsating {
  animation: pulse-animation 1.5s infinite;
}

@keyframes pulse-animation {
  1%,
  100% {
    opacity: 1;
    transform: scale(1);
  }
  50% {
    opacity: 0.5;
    transform: scale(1.4);
  }
}
.decorations2 {
  display: inline-block;
  animation: pulse 1.5s infinite;
  margin: 0 8px;
}

@keyframes pulse {
  0% {
    transform: scale(1);
    color: #ff0000;
  }
  25% {
    transform: scale(1.1);
    color: #00ff00;
  }
  50% {
    transform: scale(1);
    color: #0000ff;
  }
  75% {
    transform: scale(1.1);
    color: #ff00ff;
  }
  100% {
    transform: scale(1);
    color: #ff0000;
  }
}

.decorations2 a {
  text-decoration: none;
  transition: color 0.3s;
}

.decorations2 a:hover {
  color: #ff0000;
}

@media (max-width: 941px) {
  .container {
    height: 100vh;

    &__img {
      display: none;
    }

    &__title {
      width: 100%;
      padding: 0 10px;
    }
    &__title-text {
      font-size: 30px;
    }
  }
}

@media (max-width: 490px) {
  .container__location-icon2 {
    width: 300px;
  }
}
@media (max-width: 375px) {
  .container {
    padding-bottom: 50px;
  }
}
</style>

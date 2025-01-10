<template>
  <div class="container" id="section3">
    <h2 class="container__title">Обо мне</h2>

    <div class="container__item">
      <div class="container__text">
        <p>
          Всем привет, меня зовут Никита. Я впервые столкнулся с программированием в университете
          <a href="https://mpei.ru/Pages/default.aspx" target="_blank"> (НИУ "МЭИ")</a>, где мы
          решали задачи на Python и Pascal. Если Python еще как-то мог привлечь, то Pascal надолго
          отбил у меня желание заниматься программированием.
        </p>
        <br />
        <p>
          Хотя уже тогда я был сильно вовлечен в мир программирования, к сожалению, вуз имел уклон в
          инженерии, а у меня была специальность в энергетике, поэтому я так и не смог полностью
          попробовать себя в кодинге.
        </p>
        <br />
        <p>
          Спустя пару лет, находясь на фрилансе, я познакомился с версткой, а затем и с
          фронтенд-разработкой. Я понял, что это именно то, что мне нужно. Мне нравится визуальная
          часть работы, ведь когда ты что-то делаешь, сразу видишь результат своих изменений.
          Процесс создания красивых и интерактивных интерфейсов вдохновляет меня и дает большое
          удовольствие.
        </p>
        <br />
        <p>
          Немного о себе: Я много путешествовал и жил в пяти странах, более года: Южная Корея ,
          Польша , а также пару месяцев в Литве , Израиле и Беларуси .
        </p>
        <br />
        <p>
          Шесть лет занимался боксом (1 разряд) и четыре года легкой атлетикой. Я веду здоровый
          образ жизни и страстно увлечен новыми технологиями.
        </p>
      </div>
      <div class="survey">
        <h3>Анкета</h3>
        <div class="survey__field">
          <span>Возраст:</span>
          <p>26 лет</p>
        </div>
        <div class="survey__field">
          <span>Образование:</span>
          <p>Бакалавр энергетики</p>
        </div>
        <div class="survey__field">
          <span>Опыт работы:</span>
          <p>3 года в фронтенд-разработке</p>
        </div>
        <div class="survey__field">
          <span>Используемые технологии:</span>
          <p>JavaScript, Vue.js, HTML, CSS</p>
        </div>
        <div class="survey__field">
          <span>Увлечения:</span>
          <p>Путешествия, спорт, технологии</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.container {
  // width: 100%;
  margin: 0 auto;
  box-sizing: border-box;
  background-color: #d1d5db;
  display: flex;
  flex-direction: column;
  align-items: center;
  &__title {
    font-size: 20px;
    padding: 0 10px;
    font-weight: lowercase;
    color: #d1d5db;
    background-color: #374151;
    border-radius: 12px;
    margin-bottom: 16px;
    margin-top: 10px;
  }
  &__text {
    display: flex;
    flex-direction: column;
    justify-content: left;
    font-size: 16px;
    font-weight: lowercase;
    color: #000000;
    width: 584px;
    height: 634px;
  }
  &__item {
    display: flex;
    justify-content: space-between;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    padding: 10px;
    margin-bottom: 20px;
  }
}
.survey {
  margin-top: 20px;
  padding: 15px;
  // display: flex;
  // flex-direction: column;
  // align-items: center;

  // background-color: #ffffff;

  width: 584px;

  h3 {
    margin-bottom: 15px;
    color: #374151;
  }

  &__field {
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;

    span {
      font-weight: bold;
      color: #374151;
    }

    p {
      margin: 0;
      color: #333333;
    }
  }
}
a {
  text-decoration: none;
  color: #b40ce7;
}
</style>

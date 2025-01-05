<template>
  <div class="container" id="section3">
    <h2 class="container__title">Обо мне</h2>
    <div class="container__text">
      <p>
        Всем привет, меня зовут Никита. Я впервые столкнулся с программированием в университете (НИУ
        "МЭИ"), где мы решали задачи на Python и Pascal. Если Python еще как-то мог привлечь, то
        Pascal надолго отбил у меня желание заниматься программированием.
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
        часть работы, ведь когда ты что-то делаешь, сразу видишь результат своих изменений. Процесс
        создания красивых и интерактивных интерфейсов вдохновляет меня и дает большое удовольствие.
      </p>
      <br />
      <p>
        Немного о себе: Я много путешествовал и жил в пяти странах, более года: Южная Корея , Польша
        , а также пару месяцев в Литве , Израиле и Беларуси .
      </p>
      <br />
      <p>
        Шесть лет занимался боксом (1 разряд) и четыре года легкой атлетикой. Я веду здоровый образ
        жизни и страстно увлечен новыми технологиями.
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.container {
  width: 100%;
  // height: 100vh;
  margin: 0 auto;
  padding: 0 20px;
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
}
</style>

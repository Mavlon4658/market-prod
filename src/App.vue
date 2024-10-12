<script>
import Header from "@/components/Header.vue"
export default {
  components: {
    Header
  },
  data () {
    return {}
  }
}
</script>

<template>
  <div class="wrapper">
    <Header />
    <div class="container">
      <ul class="breadcrumb">
        <li>
          <a href="#" class="breadcrumb__link active">Главная</a>
        </li>
        <li>
          <a href="#" class="breadcrumb__link">Прибыль за периоды</a>
        </li>
        <li>
          <a href="#" class="breadcrumb__link">Автомат. поставки</a>
        </li>
        <li>
          <a href="#" class="breadcrumb__link">Отслеживание позиций</a>
        </li>
        <li>
          <a href="#" class="breadcrumb__link">Настройки</a>
        </li>
      </ul>
      <div class="summary">
        <h3 class="summary__title">Сводные данные</h3>
        <ul class="summary__list">
          <li class="summary__list_item bg-lightblue">
            <p>Товаров меньше чем <br> на 30 дней продаж</p>
            <h4>29 шт</h4>
            <div class="summary__list_item__bottom">
              <h5>Логистика</h5>
              <a href="#">Подробнее</a>
            </div>
          </li>
          <li class="summary__list_item bg-lightblue">
            <p>Рекламные расходы 05.10.2024</p>
            <h4>25 568 ₽</h4>
            <div class="summary__list_item__bottom">
              <h5>Продвижение</h5>
              <a href="#">Подробнее</a>
            </div>
          </li>
          <li class="summary__list_item">
            <p>
              <span>Товары без движения</span>
              <img :src="this.$getImage('warning.svg')" alt="">
            </p>
            <div class="summary__list_item__bottom">
              <h5>Скоро появится</h5>
              <a href="#">Подробнее</a>
            </div>
          </li>
          <li class="summary__list_item">
            <p>
              <span>Оценка ниже 4</span>
              <img :src="this.$getImage('warning.svg')" alt="">
            </p>
            <div class="summary__list_item__bottom">
              <h5>Скоро появится</h5>
              <a href="#">Подробнее</a>
            </div>
          </li>
          <li class="summary__list_item">
            <p>
              <span>Процент выкупа</span>
              <img :src="this.$getImage('warning.svg')" alt="">
            </p>
            <div class="summary__list_item__bottom">
              <h5>Скоро появится</h5>
              <a href="#">Подробнее</a>
            </div>
          </li>
        </ul>
      </div>
      <div class="statistic">
        <div class="statistic__left">
          <div class="statistic__title">Статистика  за день</div>
          <div class="statistic__radio">
            <label for="day1">
              <input type="radio" name="day" id="day1">
              <span>Вчера</span>
            </label>
            <label for="day2">
              <input type="radio" name="day" id="day2">
              <span>Позавчера</span>
            </label>
          </div>
          <ul class="statistic__card">
            <li class="statistic__card_item">
              <h4>Заказы</h4>
              <h3>29 шт</h3>
              <div>
                <p><span class="text-red">- 23 945</span> от прошл. дня</p>
                <p><span class="text-green">+ 44 353</span> от прошл. недели</p>
              </div>
            </li>
            <li class="statistic__card_item">
              <h4>Рекламные расходы</h4>
              <h3>25 568 ₽</h3>
              <div>
                <p><span class="text-red">- 23 945</span> от прошл. дня</p>
                <p><span class="text-green">+ 44 353</span> от прошл. недели</p>
              </div>
            </li>
            <li class="statistic__card_item bg-yellow">
              <h4>Прогнозная прибыль </h4>
              <h3>25 568 ₽</h3>
              <div>
                <p><span class="text-red">- 23 945</span> от прошл. дня</p>
                <p><span class="text-green">+ 44 353</span> от прошл. недели</p>
              </div>
            </li>
          </ul>
          <div class="statistic__form">
            <div class="statistic__form_item">
              <label for="">
                <span>ФОТ за текущий месяц</span>
                <img :src="this.$getImage('warning-gray.svg')" alt="">
              </label>
              <div class="form_inp">
                <input type="text" placeholder="0 ₽ по умолчанию">
                <img :src="this.$getImage('edit.svg')" alt="">
              </div>
            </div>
            <div class="statistic__form_item">
              <label for="">
                <span>Расходы на продвижение за текущий день</span>
                <img :src="this.$getImage('warning-gray.svg')" alt="">
              </label>
              <div class="form_inp">
                <input type="text" placeholder="0 ₽ по умолчанию">
                <img :src="this.$getImage('edit.svg')" alt="">
              </div>
            </div>
          </div>
        </div>
        <div class="statistic__right">
          <img :src="this.$getImage('to-left.svg')" alt="">
          <div class="statistic__right_card">
            <h3>Прогнозная прибыль очень важный показатель как идут у вас продажи</h3>
            <p>Например:</p>
            <ul>
              <li>Вошли в акцию — проверяйте, увеличилась ли прогнозная прибыль. Если нет, лучше выйти из акции</li>
              <li>Подняли рекламную ставку — смотрите на прогнозную прибыль. Если она уменьшилась, стоит пересмотреть ставку</li>
            </ul>
            <h4>Ежедневный контроль прогнозной прибыли</h4>
            <p>—  ключ к успеху вашего бизнеса</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
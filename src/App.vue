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
    </div>
  </div>
</template>
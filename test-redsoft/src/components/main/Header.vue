<template>
  <header class="header">
    <div class="header__logo">
      <img :src="`img/${logo}`" alt />
    </div>
    <menu class="header-menu">
      <ul class="header-menu__list">
        <li class="header-menu__item">
          <a href class="header-menu__link">О сервисе</a>
        </li>
        <li class="header-menu__item">
          <a href class="header-menu__link">Функции</a>
        </li>
        <li class="header-menu__item">
          <a href class="header-menu__link">Возможности</a>
        </li>
        <li class="header-menu__item">
          <a href class="header-menu__link">Партнеры</a>
        </li>
      </ul>
    </menu>
    <nav class="header-request">
      <a href class="header-request__link">Оставить заявку</a>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    logo: String
  }
};
</script>

<style lang="sass">
.header
  display: flex
  align-items: center
  justify-content: space-between
  max-width: 1160px
  margin: auto
  position: fixed
  top: 0
  left: 0
  right: 0
  width: 100%
  padding: 10px 0
.header-menu__list
  display: flex
  align-items: center
  justify-content: center
  list-style: none
.header-menu__item
  margin-right: 50px
.header-menu__link,
.header-request__link
  color: #fff
  font-weight: 500
  text-decoration: none
.header-request
  padding: 20px 34px
  border-radius: 30px
  border: 2px solid #5489c3
</style>

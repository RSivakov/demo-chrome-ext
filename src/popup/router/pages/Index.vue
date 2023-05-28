<template>
<div>
      <!--контейнер, содержащий название, логотип и номер версии-->
    <div class="modal-header">
      <h1 class="logo">
        <img class="logo-icon" src="images/tproger-logo.png"> Запускатор Tproger
        <span class="version">(1.0.0)</span>
    </h1>
    </div>
    <!--Конец контейнера-->
    <!--контейнер, содержащий описание функций расширения-->
    <div class="modal-content">
      <p>Быстрый доступ к контентным площадкам Типичного Программиста</p>
    </div>
    <!--Конец контейнера-->
    <!--контейнер, содержащий контейнеры с иконками-->
    <div class="modal-icons">
      <div class="flex-container">
        <div class="flex">
          <!--target="_blank" — это служит для открытия новой вкладки при клике по иконке-->
          <a href="#" target="_blank">
            <i class="fa fa-globe"></i>
          </a>
        </div>
        <div class="flex">
          <a href="#" target="_blank">
            <i class="fa fa-telegram"></i>
          </a>
        </div>
        <div class="flex">
          <a href="#" target="_blank">
            <i class="fa fa-facebook"></i>
          </a>
        </div>
        <div class="flex">
          <a href="#" target="_blank">
            <i class="fa fa-vk"></i>
          </a>
        </div>
      </div>
    </div>
    <!--Конец контейнера-->
  </div>
</template>

<script>
// import Vue from 'vue';
// import App from './App';
// import store from '../store';
// import router from './router';

// global.browser = require('webextension-polyfill');
// Vue.prototype.$browser = global.browser;

// /* eslint-disable no-new */
// new Vue({
//   el: '#app',
//   store,
//   router,
//   render: h => h(App),
// });
</script>

<style>
  /* Модальная структура документа */
  /*общие настройки для всего документа*/
  html,
  body {
    font-family: 'Open Sans', sans-serif;
    font-size: 14px;
    margin: 0;
    min-height: 180px;
    padding: 0;
    width: 380px;
  }
  /*задаём настройки для заголовков первого уровня*/
  h1 {
    font-family: 'Menlo', monospace;
    font-size: 22px;
    font-weight: 400;
    margin: 0;
    color: #2f5876;
  }
  a:link,
  a:visited {
    color: #000000;
    outline: 0;
    text-decoration: none;
  }
  /*задаём ширину картинки*/
  img {
    width: 30px; /*ширина изображений*/
  }
  .modal-header {
    align-items: center; /*выравнивание элементов по центру*/
    border-bottom: 0.5px solid #dadada; /*свойства нижней разделительной линии*/
    height: 50px;
  }
  .modal-content {
    padding: 0 22px; /*отступы сверху и снизу, сверху и слева*/
  }
  .modal-icons {
    border-top: 0.5px solid #dadada; /*свойства верхней разделительной линии*/
    height: 50px;
    width: 100%;
  }
  .logo {
    padding: 16px; /*отступы со всех сторон*/
  }
  .logo-icon {
    vertical-align: text-bottom; /*выравнивание по нижней части текста*/
    margin-right: 12px; /*задётся отступ элементов от изображения*/
  }
  .version {
    color: #444;
    font-size: 18px;
  }
  .flex-container {
    display: flex; /*отображает контейнер в виде блочного элемента*/
    justify-content: space-between; /*равномерное выравнивание элементов*/
    padding: 10px 22px;
  }
  /*задаём настройки для контейнеров с иконками*/
  .flex {
    opacity: 1; /*параметр непрозрачности иконок*/
    width: 120px;
  }
  .flex:hover {
    opacity: 0.4; /*уровень непрозрачности при наведении курсора на элемент*/
  }
  .flex .fa {
    font-size: 40px;
    color: #2f5876;
  }
</style>
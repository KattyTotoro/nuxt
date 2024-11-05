<template>

    <h1>Hello from index page</h1>


    <header></header>

    <div class="tabs">

        <div class="tab">
            <input type="radio" id="tab1" name="tab-group" checked>
            <label for="tab1" class="tab-title">Главная</label>
            <section class="tab-content">Главная</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab2" name="tab-group">
            <label for="tab2" class="tab-title">Статьи</label>
            <section class="tab-content">Статьи</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab3" name="tab-group">
            <label for="tab3" class="tab-title">Видео</label>
            <section class="tab-content">Видео</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab4" name="tab-group">
            <label for="tab4" class="tab-title">Музыка</label>
            <section class="tab-content">Музыка</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab5" name="tab-group">
            <label for="tab5" class="tab-title">Рецепты</label>
            <section class="tab-content">Рецепт</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab6" name="tab-group">
            <label for="tab6" class="tab-title">Путешествия</label>
            <section class="tab-content">Путешествия</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab7" name="tab-group">
            <label for="tab7" class="tab-title">Подкаст</label>
            <section class="tab-content">Подкаст</section>
        </div>

    </div>

</template>



<style>
* {
    margin: 0;
}

header {
    height: 400px;
    background: url(img/sky.jpg) top/cover no-repeat;
}

/* Все вкладки */
.tabs {
    /* Относительное позиционирование */
    position: relative;
    top: -48px;

    margin-left: 200px;
    /* margin-right: 143px; */
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 1.2rem;
}

/* Вкладка, заголовок вкладки */
.tab,
.tab-title {
    /* Выстраиваем по горизонтали */
    display: inline-block;
}

/* Вкладка */
.tab input[type="radio"] {
    display: none;
}

/* Заголовок вкладки */
.tab-title {
    width: 200px;
    /* Цвет фона */
    background: #dfeffe78;
    /* Поля вокруг текста */
    padding: 10px 10px;
    /* Параметры рамки */
    border: 3px solid #dfeffe;
    border-radius: 10px 10px 0 0;
    /* Снизу линию убираем */
    border-bottom: none;
    text-align: center;
    box-shadow: 0 0 20px whitesmoke;
}

/* Содержимое вкладки */
.tab-content {
    height: 800px;
    /* Абсолютное позиционирование */
    position: absolute;
    /* Параметры рамки */
    border: 2px solid #dfeffe;
    /* Поля вокруг текста */
    padding: 10px;
    /* Размещаем у левого края */
    left: 0;
    /* Ширина содержимого */
    width: calc(100% - 22px);
    /* Прячем вкладку */
    display: none;
    box-shadow: 0 0 20px rgb(134, 134, 134);
}

.tab :checked+.tab-title {
    /* Относительное позиционирование */
    position: relative;
    /* Цвет фона */
    background: #fff;
    /* Сдвигаем вниз */
    top: 2px;
    /* Отображаем поверх содержимого */
    z-index: 1;
}

.tab :checked~.tab-content {
    /* Показываем активную вкладку */
    display: block;
}

/* Источник с вкладками: https://webref.ru/layout/pseudo-class-checked/tabs */
/* Полезная ссылка: http://swiperjs.com/ */
</style>

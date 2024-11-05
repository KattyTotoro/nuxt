<template>

    <h1>Hello from index page</h1>


    <header></header>

    <div class="tabs">

        <div class="tab">
            <input type="radio" id="tab1" name="tab-group" checked>
            <label for="tab1" class="tab-title">Главная</label>
            <section class="tab-content">Один</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab2" name="tab-group">
            <label for="tab2" class="tab-title">Статьи</label>
            <section class="tab-content">Два</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab3" name="tab-group">
            <label for="tab3" class="tab-title">Видео</label>
            <section class="tab-content">Три</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab4" name="tab-group">
            <label for="tab4" class="tab-title">Музыка</label>
            <section class="tab-content">Четыре</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab5" name="tab-group">
            <label for="tab5" class="tab-title">Рецепты</label>
            <section class="tab-content">Пять</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab6" name="tab-group">
            <label for="tab6" class="tab-title">Путешествия</label>
            <section class="tab-content">Шесть</section>
        </div>

        <div class="tab">
            <input type="radio" id="tab7" name="tab-group">
            <label for="tab7" class="tab-title">Подкаст</label>
            <section class="tab-content">Семь</section>
        </div>

    </div>

</template>



<style>
* {
    margin: 0;
}

header {
    height: 300px;
    background: url(img/sky.jpg) top/cover no-repeat;
}

.tabs {
    position: relative;
    /* Относительное позиционирование */
    margin-left: 200px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 1.2rem;
}

.tab,
.tab-title {
    display: inline-block;
    /* Выстраиваем по горизонтали */
}

.tab input[type="radio"] {
    display: none;
}

.tab-title {
    width: 200px;
    background: #dfeffe;
    /* Цвет фона */
    padding: 10px 10px;
    /* Поля вокруг текста */
    border: 1px solid #666;
    /* Параметры рамки */
    border-bottom: none;
    /* Снизу линию убираем */
    border-radius: 10px 10px 0 0;
    text-align: center;
}

.tab-content {
    height: 800px;
    position: absolute;
    /* Абсолютное позиционирование */
    border: 1px solid #666;
    /* Параметры рамки */
    padding: 10px;
    /* Поля вокруг текста */
    left: 0;
    /* Размещаем у левого края */
    width: calc(100% - 20px);
    /* Ширина содержимого */
    display: none;
    /* Прячем вкладку */
}

.tab :checked+.tab-title {
    position: relative;
    /* Относительное позиционирование */
    background: #fff;
    /* Цвет фона */
    top: 1px;
    /* Сдвигаем вниз */
    z-index: 1;
    /* Отображаем поверх содержимого */
}

.tab :checked~.tab-content {
    display: block;
    /* Показываем активную вкладку */
}

/* https://webref.ru/layout/pseudo-class-checked/tabs */
</style>

<template>

    <h1>Hello from index_2 page</h1>


    <header></header>

    <nav>
        <ul>
            <li><a href="#">Главная</a></li>
            <li><a href="#">Статьи</a></li>
            <li><a href="#">Видео</a></li>
            <li><a href="#">Музыка</a></li>
            <li><a href="#">Рецепты</a></li>
            <li><a href="#">Путешествия</a></li>
            <li><a href="#">Подкаст</a></li>
        </ul>
    </nav>

    <div class="topMenu">

        <button class="topMenuButton"><a href="#">Главная</a></button>
        <button class="topMenuButton"><a href="#">Статьи</a></button>
        <button class="topMenuButton"><a href="#">Видео</a></button>
        <button class="topMenuButton"><a href="#">Музыка</a></button>
        <button class="topMenuButton"><a href="#">Рецепты</a></button>
        <button class="topMenuButton"><a href="#">Путешествия</a></button>
        <button class="topMenuButton"><a href="#">Подкаст</a></button>

        
    </div>

    <footer>
        <div>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Rerum omnis in neque quia accusamus ex tempore
            pariatur illum officiis dolores quisquam nam facere, quaerat culpa id minus? Perspiciatis, quos. Corrupti!
        </div>
    </footer>

</template>



<style>
* {
    margin: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

header {
    width: 100%;
    height: 300px;
    background: url(img/sky.jpg) top/cover no-repeat fixed;
}

/* Навигация-меню слева */
nav {
    position: absolute;
    background: #dfeffe78;
    font-size: 1.1rem;
    margin-top: 30px;
    padding: 20px 30px 20px 0;
    border-radius: 0 8px 8px 0;
    box-shadow: 0 0 20px rgb(134, 134, 134);
}

nav ul {
    list-style-type: none;
    padding-left: 20px;
}

nav li {
    margin-top: 10px;
}

nav ul a, .topMenuButton a {
    text-decoration: none;
    color: rgb(40, 65, 91);
}

/* Все кнопки меню */
.topMenu {
    /* Относительное позиционирование */
    position: relative;
    top: -55px;
    margin-left: 200px;
    margin-right: 150px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 1.5rem;
}

/* Заголовок кнопки */
.topMenuButton {
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
    font-size: 1.5rem;

}

/* Содержимое вкладки */
.tab-content {
    height: 800px;
    /* Абсолютное позиционирование */
    position: absolute;
    /* Параметры рамки */
    border: 2px solid #dfeffe;
    border-radius: 5px;
    /* Поля вокруг текста */
    padding: 20px;
    /* Размещаем у левого края */
    left: 0;
    /* Ширина содержимого */
    width: 100%;
    /* Прячем вкладку */
    display: none;
    box-shadow: 0 0 20px rgb(134, 134, 134);
    overflow: auto;
}

.tab-content div {
    background: rgba(205, 241, 253, 0.729);
    max-width: 80%;
    margin-left: 100px;
    margin-top: 20px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 20px rgb(134, 134, 134);
}

footer {
    width: 100%;
    padding: 20px;
    background: rgba(123, 166, 194, 0.797);
    height: 200px;
    position: absolute;
    top: 150%;
    box-shadow: 0 0 20px rgb(134, 134, 134);
    border-radius: 10px 10px 0 0;
}

/* Источник с вкладками: https://webref.ru/layout/pseudo-class-checked/tabs */
/* Полезная ссылка: http://swiperjs.com/ */
</style>

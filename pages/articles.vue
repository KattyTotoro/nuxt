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

        <button class="topMenuButton"><a href="/pages/index2.vue">Главная</a></button>
        <button class="topMenuButton" style="background: #fff"><a href="#">Статьи</a></button>
        <button class="topMenuButton"><a href="#">Видео</a></button>
        <button class="topMenuButton"><a href="#">Музыка</a></button>
        <button class="topMenuButton"><a href="#">Рецепты</a></button>
        <button class="topMenuButton"><a href="#">Путешествия</a></button>
        <button class="topMenuButton"><a href="#">Подкаст</a></button>

        
    </div>

    <div>
    
        <section class="content">
                <h1>Статьи</h1>

                <div>
                    <h2>Статья 1</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                    <br>
                    <a href="#">Подробнее</a>
                </div>

               <div>
                    <h2>Статья 2</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>

                <div>
                    <h2>Статья 3</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>

                <div>
                    <h2>Статья 4</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>

                <div>
                    <h2>Статья 5</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>
                <div>
                    <h2>Статья 6</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>
                <div>
                    <h2>Статья 7</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>
                <div>
                    <h2>Статья 8</h2>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam adipisci veniam error fugit nemo,
                    reprehenderit consequatur eligendi molestiae beatae similique amet officia quidem recusandae,
                    quaerat sunt nam non dolores blanditiis.
                </div>

            </section>

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
    padding: 10px 10px;
}

/* Все кнопки меню */
.topMenu {
    /* Относительное позиционирование */
    position: relative;
    top: -55px;
    margin-left: 200px;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    font-size: 1.5rem;
    z-index: 2;
}

/* Заголовок кнопки */
.topMenuButton {
    width: 200px;
    background: #dfeffe78;
    padding: 10px 10px;
    border: 3px solid #dfeffe;
    border-radius: 10px 10px 0 0;
    box-shadow: 0 0 20px whitesmoke;
    border-bottom: none;
    text-align: center;
    font-size: 1.5rem;
}

.topMenuButton:hover {
    cursor: pointer;
}

/* Содержимое вкладки */
.content {
    /* height: 800px; */
    position: absolute;
    top: 39%;
    margin-left: 200px;
    margin-right: 150px;
    border: 2px solid #dfeffe;
    box-shadow: 0 20px 30px rgb(134, 134, 134);
    border-top: none;
    padding: 20px;
    /* width: 100%; */
    /* overflow: auto; */
}

.content div {
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

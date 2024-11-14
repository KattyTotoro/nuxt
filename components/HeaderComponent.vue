<template>

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

    <NuxtLink class="topMenuButton" :class="route.path=='/'?'currentLink':''" href="/">Главная</NuxtLink>
    <NuxtLink class="topMenuButton" :class="route.path=='/articles'?'currentLink':''" href="/articles">Статьи</NuxtLink>
    <button class="topMenuButton"><a href="#">Видео</a></button>
    <button class="topMenuButton"><a href="#">Музыка</a></button>
    <button class="topMenuButton"><a href="#">Рецепты</a></button>
    <button class="topMenuButton"><a href="#">Путешествия</a></button>
    <button class="topMenuButton"><a href="#">Подкаст</a></button>


</div>

</template>

<script setup>
const route = useRoute()
</script>
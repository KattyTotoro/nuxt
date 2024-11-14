<template>

<header></header>

<nav>
    <ul>
        <li><NuxtLink :class="route.path=='/'?'currentLink':''" href="/">Главная</NuxtLink></li>
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
    <NuxtLink class="topMenuButton" :class="route.path=='/videos'?'currentLink':''" href="/videos">Видео</NuxtLink>
    <NuxtLink class="topMenuButton" :class="route.path=='/music'?'currentLink':''" href="/music">Музыка</NuxtLink>
    <NuxtLink class="topMenuButton" :class="route.path=='/recipes'?'currentLink':''" href="/recipes">Рецепты</NuxtLink>
    <NuxtLink class="topMenuButton" :class="route.path=='/trips'?'currentLink':''" href="/trips">Путешествия</NuxtLink>
    <NuxtLink class="topMenuButton" :class="route.path=='/podcast'?'currentLink':''" href="/podcast">Подкаст</NuxtLink>


</div>

</template>

<script setup>
const route = useRoute()
</script>
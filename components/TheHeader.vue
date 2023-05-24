<template>
  <div class="header container_all">
    <ul class="header__container">
      <li><NuxtLink to="#about">Обо мне</NuxtLink></li>
      <li><NuxtLink to="#gallery">Галлерея</NuxtLink></li>
      <li class="header__logo">LOM<span>A</span>NOV<span>A</span></li>
      <li><NuxtLink to="#price">Прайс</NuxtLink></li>
      <li><NuxtLink to="#contacts">Контакты</NuxtLink></li>
    </ul>
    <div class="header__mobile">
      <div class="row">
        <div class="header__logo">LOM<span>A</span>NOV<span>A</span></div>
        <button class="burger" @click="showMenu = !showMenu" :class="showMenu ? 'hide' : 'show'">
          <svg xmlns="http://www.w3.org/2000/svg" width="32" height="32" viewBox="0 0 24 24"><path fill="transparent" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 17h14M5 12h14M5 7h14"/></svg>
        </button>
      </div>
      <ul class="header__container--mobile" v-if="!showMenu">
        <li><NuxtLink to="#about" @click="showMenu = !showMenu">Обо мне</NuxtLink><div class="line"></div></li>
        <li><NuxtLink to="#gallery" @click="showMenu = !showMenu">Галлерея</NuxtLink><div class="line"></div></li>
        <li><NuxtLink to="#price" @click="showMenu = !showMenu">Прайс</NuxtLink><div class="line"></div></li>
        <li><NuxtLink to="#contacts" @click="showMenu = !showMenu">Контакты</NuxtLink><div class="line"></div></li>
      </ul>
    </div>
  </div>
</template>
<script setup>
const showMenu = ref(true)
</script>
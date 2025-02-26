<template>
  <div>
    <div class=header>
      <ul class=header-list>
        <img class=logo src="../assets/images/header-logo.png" alt="">
        <li>
          <NuxtLink to="/" class="text-btn">Главная</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/menu" class="text-btn">Меню</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/afisha" class="text-btn">Афиша</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/cooperation" class="text-btn">Сотрудничество</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/gallery" class="text-btn">Галерея</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/news" class="text-btn">Новости</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/booking" class="btn-booking">Бронирование</NuxtLink>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style>

</style>
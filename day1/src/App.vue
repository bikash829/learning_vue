<script setup>
import NavLogo from './components/NavLogo.vue';
import NavMenu from './components/NavMenu.vue';
import SocialItems from './components/SocialItems.vue';
</script>

<template>
  <header class="navbar">
    <!-- <div class="navbar__brand"> -->
    <!-- <a class="link_normal" href="#"><img src="#" alt="Brand Logo" class="navbar__logo"></a> -->
    <!-- <a class="link_normal" href="#">
        <h3>Brand <span>Logo</span></h3>
      </a> -->

    <!-- </div> -->
    <!-- <nav class="nav">
      <ul class="nav__list">
        <li class="nav__item"><a href="#" class="nav__link">Home</a></li>
        <li class="nav__item"><a href="#" class="nav__link">About</a></li>
        <li class="nav__item"><a href="#" class="nav__link">Services</a></li>
        <li class="nav__item"><a href="#" class="nav__link">Contact</a></li>
      </ul>
    </nav>
    <div class="social">
      <a href="#" class="social__link"><i class="fa-brands fa-facebook-f"></i></a>
      <a href="#" class="social__link"><i class="fa-brands fa-x-twitter"></i></a>
      <a href="#" class="social__link"><i class="fa-brands fa-instagram"></i></a>
    </div> -->


    <!-- using component   -->


    <NavLogo />
    <NavMenu />
    <SocialItems />
  </header>
</template>

<!-- <style scoped></style> -->
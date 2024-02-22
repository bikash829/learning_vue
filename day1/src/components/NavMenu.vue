<template>
    <nav class="nav">
        <ul class="nav__list">
            <li class="nav__item" v-for="(item, index) in navItems" :key="index">
                <a href="#" class="nav__link">{{ item }}</a>
            </li>
        </ul>
    </nav>
</template>
  
<script setup>
import { ref } from 'vue';

const navItems = ref(['Home', 'About', 'Contact', 'Services', 'Profile']);
</script>
  
  <!-- Add your CSS here -->
<style scoped>
.navbar__logo {
    width: 100px;
    /* Set your logo width */
    height: auto;
    /* Maintain aspect ratio */
}

.nav ul {
    list-style-type: none;
    display: flex;
}

.nav__item {
    /* margin-right: var(--menu-spacing); */
    font-weight: 500;
    font-size: .92rem;
    text-transform: uppercase;

}

.nav__link {
    color: var(--secondary-color);
    text-decoration: none;
    padding: 8px 20px;

}

.nav__item:hover .nav__link {
    background-color: var(--color-offblue);
    color: var(--primary-color);
    border-radius: 40px;
    box-shadow: inset 0 0 3px 0 var(--color-offblue);
    /* transition: 1000ms linear; */
}

.nav__item:first-child .nav__link {
    background-color: var(--color-offblue);
    color: var(--primary-color);
    border-radius: 40px;
}

/* Responsive styles */
@media screen and (max-width: 768px) {
    .nav {
        display: none;
    }

}
</style>
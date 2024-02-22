<template>
    <div class="social">
        <a href="#" class="social__link" v-for="(link, index) in socialLinks" :key="'social-' + index">
            <i :class="link.icon"></i>
        </a>
    </div>
</template>
  
<script setup>
import { ref } from 'vue';

const socialLinks = ref([
    { icon: 'fa-brands fa-facebook-f' },
    { icon: 'fa-brands fa-twitter' },
    { icon: 'fa-brands fa-instagram' },
]);
</script>
  
  <!-- Add your CSS here -->
<style scoped>
.social {
    display: flex;
    align-items: center;
}

.social__link {
    color: var(--secondary-color);
    text-decoration: none;
    margin-left: var(--menu-spacing);
}

/* Responsive styles */
@media screen and (max-width: 768px) {
    .nav {
        display: none;
    }

}
</style>
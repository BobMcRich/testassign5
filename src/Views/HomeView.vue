<script setup>
import { RouterLink } from 'vue-router';
import Header from '../Header.vue';

</script>

<template>
    <div>
        <button class="language-btn">English</button>
        <RouterLink to="/register" class="button register">Register</RouterLink>
        <RouterLink to="/login" class="button login">Login</RouterLink>
       <Header />
    </div>
</template>

<style scoped>

</style>
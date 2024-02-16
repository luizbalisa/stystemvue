<script setup>
import { RouterLink, RouterView } from 'vue-router'


</script>

<template>
    <nav class="nav_main">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
    </nav>
    <RouterView />
</template>

<style scoped>
.nav_main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 100%;
    background-color: #000;
    color: #f0f0f0;
    padding: 1rem;
    gap: 1rem;
	height: var(--gap-bigger);

}
</style>
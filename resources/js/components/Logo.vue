<script setup>
import { Link } from '@inertiajs/vue3';
</script>

<template>
   <Link href="/" class="text-white">
       <h1 class="logo">E-blog</h1>
   </Link>
</template>

<style scoped lang="scss">
.logo {
    font-weight: bold;
    font-size: 2rem;
    letter-spacing: 3px;
    color: $color-title;
}
</style>

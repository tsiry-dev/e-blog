<script setup>
import Logo from '@/components/Logo.vue';
import { Link, useForm } from '@inertiajs/vue3';
</script>

<template>
      <nav class="nav border-b-1 border-gray-300">
        <div class="h-[4rem] max-w-[70rem] mx-auto flex items-center justify-between ">
            <Logo />

            <ul class="flex gap-4 text-white">
                <div class="flex gap-4">
                    <Link :href="route('login')" class="nav-link">Connexion</Link>
                    <Link :href="route('register')" class="nav-link">Inscription</Link>
                </div>
            </ul>
        </div>
      </nav>
</template>

<style scoped lang="scss">
.nav {
    background: $color-white;

    &-link {
        color: $color-link;
    }
}
</style>

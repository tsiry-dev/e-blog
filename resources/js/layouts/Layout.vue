<script setup>
import { Link, useForm } from '@inertiajs/vue3';


</script>


<template>

      <nav class="bg-red-500 flex items-center justify-between h-[4rem] px-45">
        <Link href="/" class="text-white">Starter-kit</Link>

        <ul class="flex gap-4 text-white">
            <div v-if="auth?.user" class="flex gap-4">
                NAVBAR
            </div>
            <div v-else>
                <Link :href="route('login')" class="text-white">Login</Link>
            </div>
        </ul>
      </nav>

      <main class="max-w-[80rem] mx-auto mt-8">
          <slot />
      </main>
</template>

<style scoped>
</style>

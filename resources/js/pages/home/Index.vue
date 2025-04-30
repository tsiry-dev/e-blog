<script setup lang="ts">
import { Link } from '@inertiajs/vue3';
</script>

<template>
   <header class="header">
     <h1 class="header-title">Parlez de ce qui vous passionne,<br> à votre manière</h1>
     <div class="mt-15">
        <Link class="btn-primary" :href="route('login')">Créer votre blog</Link>
     </div>


     <div class="header-pic">
        <img class="header-img w-full" src="/images/bg.jpg" alt="Blog" >
     </div>
    </header>

    <section class="section about flex">
        <div class="flex-1 p-20">
            <h2 class="section-subtitle text-white">A propos de nous</h2>
            <p class="para text-white">
               Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam ratione facere temporibus exercitationem. In repellendus placeat fugiat qui quod aspernatur quos sed a aliquid unde ab, debitis sequi facere alias nostrum autem culpa consequatur praesentium eaque, veniam eligendi porro. Praesentium.
            </p>
        </div>
        <div class="flex-1 bg-yellow-500">
            <img class="h-[25rem] w-full object-cover" src="/images/bg.jpg" alt="Blog">
        </div>
    </section>
</template>

<style scoped lang="scss">
    .header {
        padding: 0 3rem 0 3rem;
        text-align: center;
        // background: $color-secondary;

        &-title {
            color: $color-title;
            font-size: 3rem;
            text-transform: uppercase;
            font-weight: bold;
        }

        &-pic {
            width: 40%;
            margin: 3rem auto;
        }

        &-img {
            width: 100%;
            height: 30rem;
            object-fit: cover;
        }
    }

    .about {
        background: $color-secondary;
    }
</style>

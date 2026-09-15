<script setup>
import { onMounted, ref } from 'vue';
import { useRouter } from 'vue-router';

const router = useRouter();
</script>

<template>
    <div>
        <header class="md:h-[700px] h-[500px] flex items-center justify-center">
            <div
                class="bg-black/50 absolute top-0 left-0 md:p-20 sm:p-10 p-2 md:pt-40 sm:pt-24 pt-20 p-6 w-full md:h-[700px] h-[500px]">

                <div class="text-white max-w-4xl max-h-[400px] bg-black/30 backdrop-blur-sm sm:p-10 p-5 rounded-3xl border border-white/20">
                    <h1 class="md:text-5xl sm:text-4xl text-2xl duration-500">Dyslexia Services & Assessments in Devon
                    </h1>
                    <p class="duration-500 font-light mt-4 text-sm sm:text-lg">I can help children and young adults throughout Newton
                        Abbot and Devon. I
                        am fully qualified and DBS
                        checked, so you can rest assured that your child is in safe hands.</p>

                    <router-link to="/contact" class="primary-button hover:bg-primary/100" role="button">Contact Me</router-link>
                </div>
            </div>
        </header>
    </div>
</template>

<style>
header {
    background-image: url('/src/assets/girl-writing.webp');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}
</style>

<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();
</script>

<template>
    <header class="relative isolate min-h-[650px] overflow-hidden bg-slate-950 md:min-h-[760px]">
        <div aria-hidden="true" class="absolute inset-0 -z-20 scale-[1.02] bg-cover bg-center bg-no-repeat backgroundimagecover"></div>

        <div aria-hidden="true"
            class="absolute inset-0 -z-10 bg-gradient-to-r from-slate-950/90 via-slate-950/60 to-slate-950/10"></div>

        <div aria-hidden="true"
            class="absolute inset-0 -z-10 bg-gradient-to-t from-slate-950/70 via-transparent to-slate-950/20"></div>

        <div aria-hidden="true"
            class="absolute inset-0 -z-10 bg-[radial-gradient(circle_at_25%_45%,transparent_0%,rgba(2,6,23,0.15)_45%,rgba(2,6,23,0.45)_100%)]">
        </div>

        <div class="mx-auto flex min-h-[650px] max-w-7xl items-center px-6 py-24 sm:px-10 md:min-h-[760px] lg:px-12">
            <section class="max-w-3xl" aria-labelledby="hero-heading">
                <div class="mb-6 flex items-center gap-3">
                    <span aria-hidden="true" class="h-px w-10 bg-white/70"></span>

                    <p class="text-xs font-medium uppercase tracking-[0.25em] text-white/80">
                        Specialist Dyslexia Support
                    </p>
                </div>

                <h1 id="hero-heading"
                    class="max-w-3xl text-4xl font-semibold leading-[1.08] tracking-[-0.03em] text-white sm:text-5xl md:text-6xl lg:text-7xl">
                    Dyslexia Services & Assessments in Devon
                </h1>

                <p class="mt-7 max-w-2xl text-base font-light leading-7 text-white/80 sm:text-lg sm:leading-8">
                    I can help children and young adults throughout Newton Abbot and Devon. I am fully qualified and DBS
                    checked, so you can rest assured that your child is in safe hands.
                </p>

                <nav aria-label="Hero actions" class="mt-9">
                    <router-link to="/contact"
                        class="group inline-flex w-fit items-center gap-3 rounded-full bg-white px-7 py-3.5 text-sm font-semibold text-slate-900 shadow-2xl shadow-black/20 transition-all duration-300 hover:-translate-y-0.5 hover:bg-white/90">
                        Get in touch

                        <svg aria-hidden="true"
                            class="h-4 w-4 transition-transform duration-300 group-hover:translate-x-1"
                            viewBox="0 0 16 16" fill="none">
                            <path d="M3 8h9M8.5 4.5 12 8l-3.5 3.5" stroke="currentColor" stroke-width="1.5"
                                stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                    </router-link>
                </nav>

                <ul class="mt-12 flex flex-wrap items-center gap-x-8 gap-y-4 border-t border-white/15 pt-6"
                    aria-label="Service credentials">
                    <li>
                        <p class="text-sm font-medium text-white">Fully Qualified</p>
                        <p class="mt-0.5 text-xs text-white/50">Professional assessment</p>
                    </li>

                    <li aria-hidden="true" class="hidden h-8 w-px bg-white/15 sm:block"></li>

                    <li>
                        <p class="text-sm font-medium text-white">DBS Checked</p>
                        <p class="mt-0.5 text-xs text-white/50">Safe & trusted service</p>
                    </li>

                    <li aria-hidden="true" class="hidden h-8 w-px bg-white/15 sm:block"></li>

                    <li>
                        <p class="text-sm font-medium text-white">Newton Abbot & Devon</p>
                        <p class="mt-0.5 text-xs text-white/50">Local support</p>
                    </li>
                </ul>
            </section>
        </div>

        <div aria-hidden="true"
            class="absolute bottom-0 left-0 right-0 h-24 bg-gradient-to-t from-slate-950 to-transparent"></div>
    </header>
</template>

<style>
.backgroundimagecover {
    background-image: url('../../src/assets/girl-writing.webp');
}
</style>
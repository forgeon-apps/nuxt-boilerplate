<script setup lang="ts">
const { t } = useI18n()

useHead({
  title: t('pages.minimal.meta.title'),
  meta: [{ name: 'description', content: t('pages.minimal.meta.description') }],
})

useSeoMeta({
  title: t('pages.minimal.meta.title'),
  description: t('pages.minimal.meta.description'),
})

definePageMeta({
  layout: 'fullscreen',
})
</script>

<template>
  <div class="min-h-screen bg-black px-4 py-6 text-neutral-100 sm:px-8 sm:py-10">
    <div class="mx-auto flex h-full max-w-3xl flex-col">
      <header>
        <h1 class="text-3xl font-semibold tracking-tight sm:text-4xl">
          {{ $t('pages.minimal.title') }}
        </h1>
      </header>

      <main
        class="mt-6 space-y-4 text-sm leading-relaxed text-neutral-400 sm:text-base"
      >
        <p v-for="index in 3" :key="index">
          {{ $t('pages.minimal.p') }}, {{ $t('pages.minimal.p') }}
        </p>
      </main>
    </div>
  </div>
</template>

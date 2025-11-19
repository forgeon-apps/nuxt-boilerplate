<script setup lang="ts">
const { t } = useI18n()

useHead({
  title: t('pages.index.meta.title'),
  meta: [{ name: 'description', content: t('pages.index.meta.description') }],
})

useSeoMeta({
  title: t('pages.index.meta.title'),
  description: t('pages.index.meta.description'),
})

definePageMeta({
  layout: 'default',
})
</script>

<template>
  <div class="flex justify-center">
    <section class="mt-10 flex w-full justify-center px-4">
      <ul
        class="grid w-full max-w-4xl grid-cols-1 gap-3 text-sm text-neutral-300 sm:grid-cols-2 md:grid-cols-3"
      >
        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:text-aa" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.googleFonts') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="simple-icons:tailwindcss" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.TailwindCSS') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="simple-icons:prettier" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.Prettier') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:cookie" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.cookies') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="streamline-logos:eslint-logo-solid" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.eslint') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:sun-horizon" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.darkMode') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:translate" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.i18n') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="simple-icons:iconify" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.Iconify') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="nonicons:typescript-16" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.Typescript') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="simple-icons:postcss" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.postcss') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:devices" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.deviceDetect') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="mdi:fruit-pineapple" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.Pinia') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:images" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.imageOptim') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:lighthouse" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.lightHouse') }}
          </div>
        </li>

        <li
          class="group flex items-center rounded-lg border border-neutral-800 bg-black/80 p-3 transition hover:border-neutral-500 hover:bg-neutral-900"
        >
          <div
            class="flex h-9 w-9 items-center justify-center rounded-md border border-neutral-700 bg-neutral-950 text-neutral-100"
          >
            <Icon name="ph:building-office" />
          </div>
          <div class="pl-3">
            {{ $t('pages.index.features.enterprise') }}
          </div>
        </li>
      </ul>
    </section>
  </div>
</template>

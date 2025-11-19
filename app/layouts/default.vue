<script setup lang="ts">
const { t } = useI18n()
</script>

<template>
  <!--
    Minimal black & white layout for playground/demo.
  -->
  <div class="min-h-screen bg-black text-neutral-100">
    <nav
      class="flex items-center justify-between border-b border-neutral-800 bg-black/90 px-4 py-3 backdrop-blur-sm sm:px-6"
      :class="t('locale.dir') === 'rtl' ? 'flex-row-reverse' : 'flex-row'"
    >
      <ul class="flex items-center gap-2">
        <li>
          <NuxtLink
            to="/"
            class="rounded-md px-3 py-2 text-xs font-medium uppercase tracking-wide text-neutral-300 transition hover:bg-neutral-900 hover:text-white"
          >
            {{ t('pages.index.link') }}
          </NuxtLink>
        </li>
        <li>
          <NuxtLink
            to="/minimal"
            class="rounded-md px-3 py-2 text-xs font-medium uppercase tracking-wide text-neutral-300 transition hover:bg-neutral-900 hover:text-white"
          >
            {{ t('pages.minimal.link') }}
          </NuxtLink>
        </li>
      </ul>

      <div class="flex items-center gap-2">
        <NuxtLink
          class="flex h-9 w-9 items-center justify-center rounded-lg text-neutral-300 transition hover:bg-neutral-900 hover:text-white"
          target="_blank"
          aria-label="Github"
          to="https://github.com/renegadevi/nuxt-boilerplate"
        >
          <Icon name="simple-icons:github" size="18" color="white" />
        </NuxtLink>

        <ThemeSwitcher
          class="rounded-lg p-2 text-neutral-300 transition hover:bg-neutral-900 hover:text-white"
        />

        <LanguageSelector />
      </div>
    </nav>

    <header class="mx-auto w-full max-w-4xl px-4 pt-10 sm:px-6">
      <div class="flex flex-col items-center gap-4 text-center">
        <Icon name="logos:nuxt-icon" size="42" />
        <div class="flex flex-col gap-2">
          <div
            class="text-xs font-semibold uppercase tracking-[0.25em] text-neutral-400"
          >
            {{ $t('pages.index.hero.subtitle') }}
          </div>
          <div class="text-3xl font-bold text-neutral-50 sm:text-4xl">
            {{ $t('pages.index.hero.title') }}
          </div>
          <div class="text-sm text-neutral-400">
            {{ $t('pages.index.hero.description') }}
          </div>
        </div>
      </div>
    </header>

    <main class="flex w-full justify-center py-10">
      <div class="container max-w-4xl px-4 sm:px-6">
        <slot />
      </div>
    </main>

    <footer
      class="border-t border-neutral-900 py-8 text-center text-xs text-neutral-500"
    >
      <p>© {{ new Date().getFullYear() }} · {{ $t('site.name') }}</p>
    </footer>
  </div>
</template>

<style lang="postcss">
ul .router-link-exact-active {
  @apply bg-neutral-100 text-black dark:bg-neutral-100 dark:text-black;
}
</style>

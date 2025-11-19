<template>
  <main
    class="flex w-full justify-center bg-black px-4 pt-8 text-neutral-100 sm:px-6 sm:pt-10"
  >
    <div class="flex w-full max-w-4xl items-start gap-4">
      <NuxtLink
        to="/"
        class="flex h-10 w-10 items-center justify-center rounded-full border border-neutral-800 text-neutral-300 transition hover:border-neutral-500 hover:bg-neutral-900 hover:text-white"
        aria-label="Back to home"
      >
        <Icon name="ph:arrow-left" size="18" />
      </NuxtLink>

      <div
        class="flex-1 border-l border-neutral-900 pl-4 sm:pl-6"
      >
        <slot />
      </div>
    </div>
  </main>
</template>

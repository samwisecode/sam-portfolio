<template>
  <div class="container mx-auto max-w-4xl">
    <header class="flex justify-between items-start md:items-center mt-5">
      <div class="flex items-center md:space-x-12">
        <div class="hidden md:block">
          <NuxtLink to="/" class="text-xl font-semibold p-2">
            <h1>Sam Norris-Rogers</h1>
          </NuxtLink>
        </div>

        <Menu />
      </div>

      <ClientOnly>
        <ColorModeSelector />
      </ClientOnly>
    </header>

    <main class="p-2 mt-10">
      <slot />
    </main>
  </div>
</template>

<script setup>
useHead({
  titleTemplate: "%s - Sam Norris-Rogers",
  link: [
    {
      rel: "preconnect",
      href: "https://fonts.googleapis.com",
    },
    {
      rel: "preconnect",
      href: "https://fonts.gstatic.com",
      crossorigin: "",
    },
    {
      rel: "stylesheet",
      href: "https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=JetBrains+Mono:ital,wght@0,100..800;1,100..800&display=swap",
      crossorigin: "",
    },
  ],
});
</script>

<style>
body {
  font-family: "Inter", sans-serif;
}

body {
  @apply bg-white dark:bg-gray-900 text-gray-700 dark:text-gray-300;
}

h1 {
  font-family: "Inter";
}
</style>

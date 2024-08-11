<template>
  <nav>
    <ul class="flex flex-col md:flex-row md:space-x-4">
      <li>
        <NuxtLink to="/" class="link">/home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/about" class="link">/about</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/projects" class="link">/projects</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/blog" class="link">/blog</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/now" class="link">/now</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
.link {
  @apply p-1 hover:text-gray-500 text-2xl md:text-base;
  font-family: "JetBrains Mono";
}
</style>

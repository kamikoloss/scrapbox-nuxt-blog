<template>
  <div class="bg-gray-100">
    <div class="w-full max-w-3xl px-8 mx-auto text-gray-900 bg-white">
      <header>
        <div class="py-32">
          <h1 class="font-bold text-2xl">
            <NuxtLink to="/">BLOG TITLE</NuxtLink>
          </h1>
          <p>Blog description hogehoge fugafuga.</p>
        </div>
      </header>
      <main>
        <slot />
      </main>
      <footer>
        <div class="py-4">
          <p class="text-center text-sm text-gray-500">Blog footer hogehoge fufafuga.</p>
        </div>
      </footer>
    </div>
  </div>
</template>

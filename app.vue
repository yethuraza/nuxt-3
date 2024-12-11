<template>
  <div class="w-screen h-screen flex justify-center items-center">
    <div class="w-[500px] h-[400px] bg-slate-300">
      <nav>
        <NuxtLink to="/">Home</NuxtLink> |
        <NuxtLink to="/movies">Movies</NuxtLink>
      </nav>
      <NuxtPage />
    </div>
  </div>
</template>

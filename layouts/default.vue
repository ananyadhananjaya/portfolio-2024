<template>
  <div class="flex flex-col min-h-screen">
    <header class="py-5 px-3 flex items-center justify-between nav-bg">
    <div>
      <NuxtLink to="/" class="nav-link p-2 px-4" exact>Ananya</NuxtLink>
    </div>
    <nav class="space-x-4">
      <NuxtLink to="/about" class="nav-link p-2 px-4">About</NuxtLink>
    </nav>
  </header>

    <div class="flex-1">
      <slot />
    </div>
    <footer class="flex justify-center py-4 mt-auto">
      <p>&copy; 2023 Ananya Dhananjaya. All Rights Reserved.</p>
    </footer>
  </div>
</template>


<style scoped>
.nav-link {
  border-radius: 24px;
  transition: background-color 0.5s;
}

.nav-link.router-link-active {
  background-color: #618264;
  color: #fff;
}

.nav-bg {
  background-color: #B0D9B1;
}
</style>
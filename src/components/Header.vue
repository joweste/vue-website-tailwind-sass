<template>
  <div class="structure">
    <header class="header">
      <a href="#" class="logo">
        <img
          class="h-7 object-cover"
          :src="require('@/assets/kusama-logo.svg')"
          alt="Kusama"
        />
      </a>
      <nav>
        <ul>
          <li><a href="#">Guide</a></li>
          <li><a href="#">Clain KSM</a></li>
          <li><a href="#">Blog</a></li>
        </ul>
        <button
          class="bg-transparent  text-red-600 text-sm  px-2 py-1 border border-red-400 rounded
           hover:text-blue-600 hover:border-blue-400 m-2 md:m-0"
        >
          Start Building
        </button>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "Header",
  data: () => ({}),
};
</script>

<style scoped src="@/assets/css/header.css"></style>

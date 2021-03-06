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

<style>
/*header*/
.header {
  display: grid;
  padding: 10px;
  grid-template-columns: minmax(130px, 1fr) auto;
  align-items: center;
}

.header nav,
.header nav ul {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.header nav ul + button {
  margin-left: var(--margin-nav-li);
}

.header li + li {
  margin-left: var(--margin-nav-li);
}
.header nav a {
  padding: 0px;
  color: rgba(255, 255, 255, 0.5);
  border-radius: 5px;
  transition: 0.1s;
}
.header nav a:hover {
  color: rgba(255, 255, 255, 0.8);
}

@media only screen and (max-width: 600px) {
  .header {
    display: block;
  }
  .header img {
    margin: 10px auto;
  }
  .header nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
}
</style>

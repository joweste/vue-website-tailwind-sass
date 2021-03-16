<template>
  <div class="structure">
    <Header />
    <Content />
    <Footer />
  </div>
  <!-- <div class="wrapper">
    <div class="card">
      <h1 class="font-bold text-6xl ">Vues With TailwindCSS v2</h1>
      <h2 class="text-3xl font-bold">Using VueCLI</h2>
    </div>
  </div> -->
</template>

<script>
import Header from "@/components/Header";
import Content from "@/components/Content";
import Footer from "@/components/Footer";
export default {
  components: { Header, Footer, Content },
};
</script>

<style lang="postcss"></style>

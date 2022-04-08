<script setup>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
</script>

<template>
  <header>
    <Header />
  </header>

  <main>
    <Main />
  </main>
</template>

<style>
@import "./assets/base.css";

header {
  width: 100%;
  max-width: 1920px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

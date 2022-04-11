<template>
  <div id="app">
    <header>
      <HeaderComponent />
    </header>
    <main>
      <MainComponent />
      <ExerciseTwo />
      <BonusQuestions />
    </main>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import ExerciseTwo from "./components/ExerciseTwo.vue";
import BonusQuestions from "./components/BonusQuestions.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    MainComponent,
    ExerciseTwo,
    BonusQuestions,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

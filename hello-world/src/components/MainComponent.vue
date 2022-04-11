<template>
  <div class="container">
    <div class="container__inner">
      <MainItem />
      <MainItem />
      <MainItem />
    </div>
  </div>
</template>

<script>
import MainItem from "./MainItem.vue";
export default {
  name: "MainComponent",
  components: {
    MainItem,
  },
};
</script>

<style scoped>
.container {
  /* width: 1920px; */
  max-width: 1920px;
  height: auto;
  margin: auto;
  padding: 50px 0;
}

.container__inner {
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0 10%;
}

@media screen and (max-width: 850px) {
  .container__inner {
    flex-direction: column;
  }
}
</style>

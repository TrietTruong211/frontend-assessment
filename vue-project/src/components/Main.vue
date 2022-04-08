<script setup>
import Item from "./Item.vue";
</script>

<template>
  <div class="container">
    <div class="container__inner">
      <Item />
      <Item />
      <Item />
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
  components: {},
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
</style>

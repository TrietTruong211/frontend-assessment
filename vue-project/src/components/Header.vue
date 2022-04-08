<template>
  <div class="container">
    <div class="container__background">
      <div class="container__inner">
        <h1 class="container__inner-content welcome-text">Hello Developer!</h1>
        <h2 class="container__inner-content secondary-text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        </h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  components: {},
};
</script>

<style scoped>
.container {
  /* width: 100%; */
  max-width: 1920px;
  width: 1920px;
  height: 500px;
  margin: auto;
}

.container__background {
  width: 100%;
  background: url(http://via.placeholder.com/1920x650);
  height: 100%;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container__inner {
  margin: auto;
}

.container__inner-content {
  color: white;
  text-align: center;
}

.welcome-text {
  font-size: 4em;
  font-weight: 700;
  /* margin-top: 20px; */
}

.secondary-text {
  font-size: 2.2em;
  margin-top: -20px;
}
</style>

<template>
  <div class="item__container">
    <div class="item__container-inner">
      <img class="item__text-image" src="http://via.placeholder.com/400x300" />
      <div class="item__text-container">
        <p class="item__text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur
          mattis sem a diam euismod egestas. Class aptent taciti sociosqu ad
          litora torquent per conubia nostra, per inceptos himenaeos. Vestibulum
          sagittis magna cursus, pharetra ex commodo, pretium mauris.
        </p>
      </div>
      <div class="item__button-container">
        <button class="item__button">Read More</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Item",
  components: {},
  props: {
    imgUrl: String,
    text: String,
  },
};
</script>

<style scoped>
.item__container {
  width: 30%;
  border: 1px solid rgba(236, 236, 236, 0.75);
  border-radius: 10px;
  box-shadow: 0 0 5px rgba(236, 236, 236, 0.75);
}

.item__container-inner {
  padding: 20px;
  border-radius: 10px;
}

.item__text-image {
  width: 100%;
  border-radius: 10px;
}

.item__text {
  color: black;
  text-align: center;
  font-weight: 400;
}

.item__button-container {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px 0;
}

.item__button {
  background: white;
  border: 4px solid black;
  border-radius: 50px;
  text-transform: uppercase;
  padding: 10px;
  font-weight: bold;
  margin: auto;
  letter-spacing: 3px;
}
</style>

<template>
  <div class="exercisetwo__container">
    <div class="exercisetwo__container-inner exercisetwo__tabs">
      <b-tabs content-class="mt-4">
        <div v-for="data in myData" v-bind:key="data.title">
          <b-tab :title="data.title" v-html="data.content"> </b-tab>
        </div>
      </b-tabs>
    </div>

    <div class="exercisetwo__container-inner exercisetwo__accordion">
      <div
        class="accordion"
        role="tablist"
        v-for="data in myData"
        v-bind:key="data.title"
      >
        <b-card no-body class="mb-1">
          <b-card-header header-tag="header" class="p-1" role="tab">
            <b-button
              block
              v-b-toggle="data.title.split(' ').join('')"
              variant="info"
              v-html="data.title"
            >
            </b-button>
          </b-card-header>
          <b-collapse
            :id="data.title.split(' ').join('')"
            visible
            accordion="my-accordion"
            role="tabpanel"
          >
            <b-card-body v-html="data.content"> </b-card-body>
          </b-collapse>
        </b-card>
      </div>
    </div>
  </div>
</template>
<script>
import data from "../assets/data.json";

export default {
  name: "ExerciseTwo",
  components: {},
  data() {
    return {
      myData: data,
    };
  },
};
</script>

<style scoped>
.exercisetwo__container {
  max-width: 1920px;
  width: 100%;
  padding: 50px 10%;
}

.exercisetwo__accordion {
  display: none;
}

@media screen and (max-width: 850px) {
  .exercisetwo__tabs {
    display: none;
  }

  .exercisetwo__accordion {
    display: block;
  }
}

.tab-pane,
.card-body {
  text-align: start;
}

.card-header {
  background-color: white;
  padding: 0 !important;
}

.accordion button {
  border-radius: initial;
  width: 100%;
  background-color: white;
  border: none;
  text-align: start;
}

.accordion .not-collapsed {
  background-color: #0d6efd;
}

.btn-info:focus,
.btn-info:hover {
  box-shadow: 0 0 0 0.25rem #0d6efd;
  border-color: #0d6efd;
}
</style>

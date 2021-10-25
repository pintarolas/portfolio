<template>
  <div class="card py-3">
    <div class="card-head">
      <img alt="Project logo" :src="image" />
      <h2>{{ title }}</h2>
    </div>
    <hr />
    <div class="card-body">
      <p>{{ description }}</p>
    </div>
    <hr />
    <div class="container">
      <div class="row">
        <div
          class="col-4 my-auto mx-auto d-block wd-100"
          v-for="framework in frameworks"
          :key="framework"
        >
          <img alt="Framework logo" class="img-fluid" :src="framework.frame" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "card",
  props: {
    title: String,
    image: String,
    description: String,
    frameworks: Array,
  },
};
</script>

<style scoped>
.row {
  height: 100px;
}
</style>


<script>
export default {
  props: {
    name: String,
    status: String,
    species: String,
    image: String

  }
}


</script>

<template>
  <div class="col mb-3 ">
    <div class="card">
      <img :src="image" class="card-img-top" :alt="name">
      <div class="card-body">
        <h4 class="card-title">{{ name }}</h4>
        <h5 class="card-title mt-3">{{ status }}</h5>
        <h5 class="card-title">{{ species }}</h5>

      </div>
    </div>
  </div>

</template>

<style lang="scss" scoped></style>
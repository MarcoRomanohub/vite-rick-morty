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
  <div class="col mb-5 ">
    <div class="card border-0 mx-3">
      <img :src="image" class="card-img-top" :alt="name">
      <div class="card-body">
        <h4 class="card-title">{{ name }}</h4>
        <h5 :class="status" class="card-title mt-3">{{ status }}</h5>
        <h5 class="card-title">{{ species }}</h5>

      </div>
    </div>
  </div>

</template>

<style lang="scss" scoped>
img {
  border-radius: 50%;
  transition: transform .2s;

  &:hover {
    transform: scale(1.1);
  }
}

.Alive {
  background-color: rgba(0, 128, 0, 0.555);
}

.Dead {
  background-color: red;
}
</style>
<script>
import { store } from '../data/store'
export default {
  data() {
    return {
      store
    }
  }
}

</script>

<template>
  <div class="container text-center my-5 ">
    <h1>{{ store.mainTitle }}</h1>
    <label for="exampleDataList" class="form-label">Ricerca per nome</label>
    <input class="form-control" list="datalistOptions" id="exampleDataList" placeholder="Type to search...">
    <datalist id="datalistOptions">
      <option value="San Francisco"></option>
      <option value="New York"></option>
      <option value="Seattle"></option>
      <option value="Los Angeles"></option>
      <option value="Chicago"></option>
    </datalist>
  </div>

</template>

<style lang="scss" scoped></style>

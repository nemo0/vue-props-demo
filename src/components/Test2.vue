
<template>
  <div>
    <h1>Vue Top Artist Countries</h1>
    <ul>
      <li v-for="(artist, x) in artists" :key="x">
        <h3>{{ artist.name }} from {{ artist.country }}</h3>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "Test",
  props: ["artists"],
};
</script>
<style scoped>
li {
  height: 40px;
  width: 100%;
  padding: 15px;
  border: 1px solid saddlebrown;
  display: flex;
  justify-content: center;
  align-items: center;
}
a {
  color: #42b983;
}
</style>
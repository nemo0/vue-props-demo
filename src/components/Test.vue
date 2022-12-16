
<template>
  <div>
    <h1>Vue Top 20 Artists</h1>
    <ul>
      <li v-for="(artist, x) in artists" :key="x">
        <h3>{{ artist.name }}</h3>
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
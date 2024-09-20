<script>
export default {
  data() {
    return {};
  },
  props: ["Thumb", "Series"],
};
</script>

<template>
  <div class="card">
    <div class="card-img mb-2">
      <img :src="Thumb" alt="img of {{ Series }}" />
    </div>
    <h2>
      {{ Series }}
    </h2>
  </div>
</template>

<style scoped>
.card {
  border: none;
  margin: 0;
  height: 100%;
  text-align: left;
  overflow: hidden;
  background-color: #222222;
}

.card-img img {
  width: 100%;
  height: 100%;
  aspect-ratio: 1;
}

h2 {
  color: white;
  background-color: #222222;
  font-size: 0.8rem;
  font-weight: 500;
  margin: 0;
}
</style>

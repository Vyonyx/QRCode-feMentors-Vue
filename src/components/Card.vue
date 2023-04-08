<script setup lang="ts">
defineProps({
  title: String,
  description: String,
  imageUrl: String,
})
</script>

<template>
  <div class="card">
    <img :src="imageUrl" :alt="description">
    <h3 class="title">{{ title }}</h3>
    <p class="description">{{ description }}</p>
  </div>
</template>

<style scoped>
.card {
  font-family: 'Outfit', sans-serif;
  max-width: 300px;
  background: white;
  padding: 1rem;
  border-radius: 1rem;
  box-shadow: 0px 20px 20px hsla(218, 44%, 22%, 0.15);
}

.card img {
  width: 100%;
  aspect-ratio: 1/1;
  border-radius: inherit;
}

.card .title {
  color: hsl(218, 44%, 22%);
  font-weight: 700;
  font-size: 1.5rem;
  font-family: inherit;
  text-align: center;
}

.card .description {
  color: hsl(220, 15%, 55%);
  font-weight: 400;
  font-size: 15px;
  font-family: inherit;
  text-align: center;
  max-width: 85%;
  margin: 0 auto;
  margin-bottom: 1rem;
}
</style>

<template>
  <div class="card">
    <img class="card-image" :src="image" :alt="title" />
    <div class="card-content">
      <h3 class="card-title">{{ title }}</h3>
      <p class="card-description">{{ description }}</p>
      <a class="card-button" :href="link">{{ button }}</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    image: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
    link: {
      type: String,
      required: true,
    },
    button: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
/* .card {
  max-width: 400px;
  border-radius: 0.5rem;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1),
    0 2px 4px -1px rgba(0, 0, 0, 0.06);
} */

.card-image {
  width: 100%;
  height: auto;
  object-fit: cover;
  border-top-left-radius: inherit;
  border-top-right-radius: inherit;
}

/* .card-content {
  padding: 1.5rem;
} */

.card-title {
  font-weight: bold;
  font-size: 1.5rem;
}

.card-description {
  margin-top: 0.5rem;
}

.card-button {
  display: inline-block;
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  border-radius: 0.25rem;
  background-color: #60a5fa;
  color: white;
}
</style>

<script setup>
import Header from "./components/Header.vue";
import Art from "./components/Art.vue";

const images = {
  image:
    "https://images.unsplash.com/photo-1531870972494-627796a756dc?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8c3VuZmxvd2VyfGVufDB8fDB8fA%3D%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60",
  title: "Sunflower",
  description:
    "A sunflower is a type of flower that belongs to the Asteraceae family. It is native to North America and has a large yellow head that follows the movement of the sun.",
  link: "https://en.wikipedia.org/wiki/Sunflower",
  button: "Learn more",
};
</script>

<template>
  <Header />
  <div class="grid grid-cols-4 gap-4 ml-16 mr-16">
    <div v-for="n in 8" class="container">
      <Art
        :image="images.image"
        :title="images.title"
        :description="images.description"
        :link="images.link"
        :button="images.button"
      />
    </div>
  </div>
</template>

<script setup>
import { RouterLink, RouterView } from "vue-router";
import { provide, ref, watchEffect } from "vue";
import ManyImgContent from "./components/ContentWithManyImg.vue";
import OneImgContent from "./components/ContentWithOneImg.vue";

const posts = ref([
  {
    title: 123123,
    user: {
      img: "",
      name: "Jerry",
      date: "2022/02/22",
    },
    content: "wordwordword",
    postImg: ["img1", "img2"],
  },
  {
    title: 123123,
    user: {
      img: "",
      name: "Jerry",
      date: "2022/02/22",
    },
    content: "wordwordword",
    postImg: ["img1"],
  },
]);
</script>

<template>
  <template v-for="post in posts">
    <div class="container">
      <ManyImgContent v-if="post.postImg.length > 1" :post="post" />
      <OneImgContent v-else :post="post"></OneImgContent>
    </div>
  </template>
</template>

<style scoped>
.container {
  padding: 5px;
  border: 1px solid black;
}
</style>

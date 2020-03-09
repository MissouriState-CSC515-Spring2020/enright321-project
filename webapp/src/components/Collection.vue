<template>
  <div class="collection">
    <div class="collection-panel" v-for="photo in photos" :key="photo.id">
      <router-link :to="`/photo/${photo.id}`">
        <img :src="thumbUrl(photo.filename)" />
      </router-link>
    </div>
  </div>
</template>

<script>
import photos from "@/photos.json";
export default {
  name: "Collection",
  data() {
    return {
      photos
    };
  },
  methods: {
    thumbUrl(filename) {
      return require(`../assets/images/${filename}`);
    }
  }
};
</script>

<style>
.collection {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(20rem, 1fr));
  grid-gap: 1rem;
  max-width: 80rem;
  margin: 5rem auto;
  padding: 0 5rem;
}
.collection-panel img {
  width: 100%;
  height: 22vw;
  object-fit: cover;
  border-radius: 0.75rem;
}
</style>
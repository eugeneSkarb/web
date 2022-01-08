<template>
  <div class="wrapper">
    <router-link class="title" :to="{name: link}">{{ title }}</router-link>
    <router-link class="title" :to="{name: link}">
      <img :src="imageSrc"
           :alt="imageAlt" class="image">
    </router-link>
  </div>
</template>

<script>
export default {
  name: "NewsElement",
  props: {
    title: String,
    imageSrc: String,
    imageAlt: String,
    link: String,
  }
}
</script>

<style scoped>
.wrapper {
  display: flex;
  flex-direction: row;
  margin-top: 40px;
  box-shadow: rgb(255 255 255) 2px 2px 2px;
  padding: 10px;
  background-color: white;
  border-radius: 10px;
}

.title {
  color: black;
  text-decoration: none;
  font-size: 18px;
  padding-right: 10px;
}

.image {
  max-height: 170px;
  max-width: 300px;
  border-radius: 10px;
}
</style>
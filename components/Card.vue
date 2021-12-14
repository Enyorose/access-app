<template>
  <div>
    <figure>
      <h3>{{ place.name }}</h3>
      <img :src="place.image_url" :alt="place.alias" width="150" height="150" />
      <figcaption></figcaption>
      <a :href="place.url"><button>More on your new favorite</button></a>
    </figure>
  </div>
</template>

<script>
export default {
  props: ["place"],
};
</script>

<style>
</style>
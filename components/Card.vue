<template>
  <div>
    <figure>
      <img :src="place.image_url" alt="" />
      <p>{{ place.name }}</p>
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
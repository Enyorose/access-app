<template>
    <figure>
      <h3>{{ place.name }}</h3>
      <img :src="place.image_url" :alt="place.alias" width="150" height="150" />
      <figcaption></figcaption>
      <a :href="place.url"><button class="btn">More on your new favorite</button></a>
    </figure>
</template>

<script>
export default {
  props: ["place"],
};

</script>

<style lang="scss">

.btn {
  @apply bg-red-500 p-2 rounded-lg m-5
}

figure {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin: 1.5rem;
  border: 1px solid gray;
  border-radius: 1rem;
  
    img {
      height: 250px;
      width: 200px;
      position: center;
      object-fit: cover;
    }

    h3 {
      font-size: 1rem;
      margin: 2rem;
    }
}



</style>
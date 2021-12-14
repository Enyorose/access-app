<template>
    <figure>
      <img :src="place.image_url" :alt="place.alias" />
      <figcaption></figcaption>
      <h3>{{ place.name }}</h3>
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
  @apply bg-red-500 p-2 rounded-lg m-6 hover:bg-red-300;
}

figure {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin: 2rem;
  box-shadow: 0px 0px 6px rgb(104, 104, 104);
  border-radius: 10px;

    img {
      height: 30vh;
      width: 100vw;
      position: center;
      object-fit: cover;
      border-radius: 10px 10px 0px 0px;
    }

    h3 {
      font-size: 18px;
      margin: 1rem;
      text-align: center;
    }
}



</style>
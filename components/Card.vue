<template>
  <figure>
    <img :src="place.image_url" :alt="place.alias" />
      <figcaption>{{ place.name }}</figcaption>
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
  @apply bg-green-400 p-2 rounded-lg m-6 hover:bg-green-600;
}

figure {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  margin: 3rem;
  border: 1px solid rgb(172, 172, 172);
  box-shadow: 0px 0px 10px rgb(119, 119, 119);
  border-radius: 10px;

    img {
      height: 30vh;
      width: 100vw;
      position: center;
      object-fit: cover;
    }

    figcaption {
      font-size: 18px;
      margin: 1rem;
      text-align: center;
      font-weight: bold;
    }
}



</style>
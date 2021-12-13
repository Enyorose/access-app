<template>
  <v-container>
    <div>
      <ul class="flex">
        <li><NuxtLink class="gap" to="/">Home</NuxtLink></li>
        <li><NuxtLink class="gap" to="/services">Services</NuxtLink></li>
        <li><NuxtLink class="gap" to="/contact">Contact</NuxtLink></li>
        <li><NuxtLink class="gap" to="/community">Community</NuxtLink></li>
      </ul>
    </div>
  </v-container>
</template>
<!-- JS -->
<script>
export default {};
</script>
<!-- CSS -->
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap');
.gap {
  @apply ml-6 mr-6 text-3xl font-bold

}
ul {
font-family: 'Kosugi Maru', sans-serif;

}



</style>
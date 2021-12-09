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

.gap {
  @apply ml-6 mr-6 text-3xl font-bold

}
ul {

color: red;
}

</style>
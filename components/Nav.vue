<template>
  <v-container>
    <div>
      <ul class="flex">
        <li>
          <NuxtLink
            to="/"
            :class="
              pageInfo.menuName === 'home' ? navClass.active : navClass.inactive
            "
            >Home</NuxtLink
          >
        </li>
        <li>
          <NuxtLink
            to="/services"
            :class="
              pageInfo.menuName === 'services'
                ? navClass.active
                : navClass.inactive
            "
            >Services</NuxtLink
          >
        </li>
        <li>
          <NuxtLink
            :class="
              pageInfo.menuName === 'contact'
                ? navClass.active
                : navClass.inactive
            "
            to="/contact"
            >Contact</NuxtLink
          >
        </li>
        <li>
          <NuxtLink
            :class="
              pageInfo.menuName === 'community'
                ? navClass.active
                : navClass.inactive
            "
            to="/community"
            >Community</NuxtLink
          >
        </li>
      </ul>
    </div>
  </v-container>
</template>
<!-- JS -->
<script>
export default {
  props: ["pageInfo"],
  data() {
    return {
      // Custom page data comes here.
      navClass: {
        active:
          "font-extrabold text-center block border-2 border-gray-300 rounded py-2 px-4 bg-emerald-500 text-indigo-600",
        inactive:
          "font-semibold text-center block border-2 border-gray-300 rounded py-2 px-4 text-blue-300 bg-white hover:text-indigo-600 hover:bg-teal-200",
      },
    };
  },
};
</script>
<!-- CSS -->
<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap"); // Cabin & Inter
@import url("https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap");

ul {
  font-family: "Kosugi Maru", sans-serif;
}
</style>
<template>
  <div>
    <nav>
      <ul>
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/services">Services</NuxtLink>
        </li>
         <li>
          <NuxtLink to="/contact">Contact</NuxtLink>
        </li>
         <li>
          <NuxtLink to="/community">Community</NuxtLink>
        </li>
      </ul>
    </nav>
    <main>
      
      <Nuxt />
    </main>
  </div>
</template>
<script>
<<<<<<< HEAD
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
=======
export default {};
>>>>>>> 7044c82c01b0a41f74f94d80956932fbb9c87349
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap"); // Cabin & Inter
@import url("https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap");
/* home route and active route will show in bold as it matches / and /about */
a.nuxt-link-active {
  font-weight: bold;
}
/* exact link will show the primary color for only the exact matching link */
a.nuxt-link-exact-active {
  color: #00c58e;
}

body {
  
  margin: 0;
}

main {
  margin: 0 auto;
  padding: 0 1rem;
  margin-top: 100px;
  max-width: 1280px;
  text-align: center;
}
img {
  margin-bottom: 1rem;
}

ul {
<<<<<<< HEAD
  font-family: "Kosugi Maru", sans-serif;
=======
    font-family: "Kosugi Maru", sans-serif;
  list-style-type: none;
  padding: 0;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
li {
  background-color: teal;
  border: solid;
  border-radius: 10px;
  border-color: indigo;
  margin: 0 0.5rem;
  padding: 0.25rem;
  font-size: 1.2rem;
  
}

nav {
  padding: 0 1rem;
>>>>>>> 7044c82c01b0a41f74f94d80956932fbb9c87349
}

a,
a:visited {
  text-decoration: none;
  color: indigo;
}

a:hover {
  color: #00c58e;
}



</style>

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
export default {};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap"); // Cabin & Inter
@import url("https://fonts.googleapis.com/css2?family=Cabin&family=Inter:wght@100&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap");
/* home route and active route will show in bold as it matches / and /about */
a.nuxt-link-active {
  
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

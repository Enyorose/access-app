<template>
  <form>
    <label for="input-search">Restaurant Name:</label>
    <input type="text" id="input-search" placeholder="Search Restaurant" />
    <div v-if="pageInfo.menuName !== 'services'" class="hidden"></div>
    <div v-else class="range">
      <label for="input-range">Search Range:</label>
      <input
        type="range"
        max="400"
        min="100"
        step="50"
        id="input-range"
        placeholder="Search Range"
      />
    </div>
    <NuxtLink to="/services"><button class="srch-btn">Search</button></NuxtLink>
  </form>
</template>
<!-- JS -->
<script>
export default {
  props: ["pageInfo"],
};
</script>
<!-- -->
<style lang="scss">
form {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 3rem;
  flex-wrap: wrap;

  label {
    font-size: 1rem;
  }

  #input-search {
    margin: 1rem;
    padding: 1rem;
    width: 300px;
    border-radius: 15px;
    border: 1px solid rgb(214, 214, 214);
  }

  .srch-btn {
    background-color: rgb(233, 233, 233);
    border: 2px solid rgb(143, 42, 42);
    padding: 10px 20px 10px 20px;
    border-radius: 15px;
  }

  .range {
    display: flex;
    align-items: center;
    margin: 1rem;

    input {
      margin: 1rem;
    }
  }

}
</style>
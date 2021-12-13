<template>
  <div>
    <div>
      <form v-on:submit.prevent="getInfo">
        <label for="input-search">Restaurant Name:</label>
        <input
          type="text"
          id="input-search"
          v-model="searchText"
          placeholder="Search Restaurant"
        />
        <label for="input-range">Search Range: {{ this.searchRange }}</label>
        <input
          type="range"
          max="400"
          min="100"
          step="50"
          id="input-range"
          v-model="searchRange"
          placeholder="Search Range"
        /><button>Search</button>
      </form>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  async asyncData() {
    const api =
      "https://api.yelp.com/v3/businesses/search?term=delis&latitude=51.06439127467012&longitude=-114.06230483054544";
    const place = await axios
      .get(api, {
        headers: {
          Authorization:
            "Bearer P7GOjS-bAd3V-QFlcM0z4Vi10A5r5i7z5Zj0j3bTxyRXdSYW6FkLyzIGrj5GIsvC0veYEtJ9EMnQplPUcOuYlH1X_lfIzLxEecGKFsqOQLEpEjC_Njk8rBQGG7GzYXYx",
        },
      })
      .then((response) => {
        console.log(response.data);
        return response.data;
      });
    return { place };
  },
  data() {
    return {
      error: "",
      searchText: "",
      searchRange: 100,
    };
  },
};
</script>

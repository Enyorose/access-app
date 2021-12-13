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
    <div v-for="place in places" :key="place.id">
      <figure>
        <img :src="place.image_url" :alt="place.alias" />
        <p>{{ place.name }}</p>
      </figure>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  async asyncData() {
    const api =
      "https://api.yelp.com/v3/businesses/search?term=delis&latitude=51.06439127467012&longitude=-114.06230483054544";
    const places = await axios
      .get(api, {
        headers: {
          Authorization: process.env.VUE_APP_API_KEY,
        },
      })
      .then((response) => {
        console.log(response.data);
        return response.data;
      });
    return { places };
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

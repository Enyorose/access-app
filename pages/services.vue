<template>
  <div>
    <Form />
    <Card v-for="place in places.businesses" :key="place.id" :place="place" />
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
          "Access-Control-Allow-Origin": "*",
          Authorization: process.env.VUE_APP_API_KEY,
        },
      })
      .then((response) => {
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

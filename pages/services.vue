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
  methods: {
    getInfo: function () {
      if (this.searchText != "") {
        axios
          .get(
            "https://cores-anywhere.herokuapp.com/https://api.yelp.com/v3/businesses/search?term=" +
              this.searchText +
              "&latitude=51.049999&longitude=-114.066666&radius=" +
              this.searchRange +
              "limit=25",
            {
              headers: {
                Authorization: process.env.API_KEY,
              },
            }
          )
          .then((res) => {
            if (res) {
              (this.restaurantList = res.data.business),
                (this.searchText = ""),
                console.log(res);
            }
          })
          .catch((err) => {
            console.log(err);
          });
      } else {
        alert("Search Bar is Empty");
      }
    },
  },
  data() {
    return {
      searchText: "",
      searchRange: 100,
      restaurantList: [],
    };
  },
};
</script>

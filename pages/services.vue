<template>
  <div>
   <div class="flex justify-between align-center p-5">
      <Header />
      <Nav />
    </div>
    <div class="search">
      <Form :pageInfo="pageInfo" />
    </div>
    <div class="wrapper">
      <Card v-for="place in places.businesses" :key="place.id" :place="place" />
    </div>
    <Footer />
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
      pageInfo: {
        menuName: "services",
        header: "Services",
      },
    };
  },
};
</script>



<style lang="scss">


.wrapper {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-auto-rows: auto;
  margin: auto;
  width: 70vw;
}

.search {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
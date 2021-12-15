<template>
  <div>
    <div class="flex justify-between align-center p-5">
      <Header />
      <Nav />
    </div>
    <!--map-->

    <div class="flex justify-evenly align-center flex-wrap m-15">
      <section class="border-2 border-gray-400 rounded-lg shadow-5xl">
        <iframe
          width="600"
          height="450"
          style="border: 0"
          loading="lazy"
          allowfullscreen
          src="https://www.google.com/maps/embed/v1/search?q=Bow%20Valley%20Square%2C%205%20Avenue%20Southwest%2C%20Calgary%2C%20AB%2C%20Canada&key=AIzaSyD6ImALDdeRhFlJaeF7P6dN33JmYNCu26c"
        ></iframe>
        <!--form-->
      </section>
      <section class="flex justify-center align-center">
        <Contactform />
      </section>
    </div>
    <Team />
  </div>
</template>
<script>
export default {
  data() {
    return {
      pageInfo: {
        menuName: "contact",
        header: "Contact",
      },
    };
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: 0;
  overflow-x: hidden;
}

</style>
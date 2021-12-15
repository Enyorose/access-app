<template>
  <div>
    <div class="flex justify-between align-center p-5">
      <Header />
      <Nav />
    </div>
    <!--map-->

    <div class="flex justify-evenly align items-center flex-wrap m-15">
         <iframe
          class="m-5"
          width="600"
          height="450"
          style="border: 0"
          loading="lazy"
          allowfullscreen
          src="https://www.google.com/maps/embed/v1/search?q=Bow%20Valley%20Square%2C%205%20Avenue%20Southwest%2C%20Calgary%2C%20AB%2C%20Canada&key=AIzaSyD6ImALDdeRhFlJaeF7P6dN33JmYNCu26c">
        </iframe>
        <!--form-->
      <section class="flex justify-center align-center m-10">
        <div class="flex text-justify flex-col text-lg">
          <p class="m-2"><strong>Email:</strong> Vebuwagroup@gmail.com</p>
          <p class="m-2"><strong>Contact:</strong> (403) 555 5555</p>
          <p class="m-2"><strong>Instagram:</strong> Vebuwa_Group </p>
        </div>
        <Contactform />
      </section>
    </div>
    <Team />
    <Footer />
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
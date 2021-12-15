<template>
  <main>
    <div class="flex justify-between align-center p-5">
      <Header />
      <Nav />
    </div>
    <!--map-->
    
    
    
    <section>
      <iframe
        width="600"
        height="450"
        style="border: 0"
        loading="lazy"
        allowfullscreen
        src="https://www.google.com/maps/embed/v1/search?q=Bow%20Valley%20Square%2C%205%20Avenue%20Southwest%2C%20Calgary%2C%20AB%2C%20Canada&key=AIzaSyD6ImALDdeRhFlJaeF7P6dN33JmYNCu26c"
      ></iframe>
      <!--form-->
      
     <Contactform />
    
    </section>
    
    <Team />
  </main>
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
section {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  text-align: center;
  align-items: center;
  align-content: center;
}
</style>
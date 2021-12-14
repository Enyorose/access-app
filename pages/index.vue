<template>
  <div class="splash">
    <div class="flex justify-between align-center p-5">
      <Header />
      <Nav :pageInfo="pageInfo" />
      
    </div>

    <article>
      <h1 class="text-5xl mb-5 md:text-6xl lg:text-8xl">A Future of Accessibilities...</h1>
      <p class="text-md md:text-xl lg:text-2xl">
        Our goal is to make your next favorite spot easy to find and suit your
        needs. </p>
        <Form :pageInfo="pageInfo" />
    </article>
    <Footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      pageInfo: {
        menuName: "home",
        header: "Home",
      },
    };
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Kosugi+Maru&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: 0;
  overflow-x: hidden;
}

.splash {
  height: 100vh;
  background-image: url(./static/assets/images/splash-page2.svg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  overflow-y: hidden ;
}

article {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  flex-direction: column;
  height: 85vh;
  padding: 2rem;
  flex-wrap: wrap;

  h1 {
  font-family: "Kosugi Maru", sans-serif;
  }

}


</style>

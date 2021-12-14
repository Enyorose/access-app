<template>
  <div class="splash">
    <div class="flex justify-between align-center p-5">
      <Header />
      <Nav :pageInfo="pageInfo" />
    </div>

    <article>
      <h1>A Future of Accessibilities...</h1>
    </article>
    <article>
      <h2>
        Our goal is to make your next favorite spot easy to find and suit your
        needs.
      </h2>
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
h1 {
  font-size: 5em;
  font-family: "Kosugi Maru", sans-serif;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: 0;
}

.splash {
  height: 100vh;
  background-image: url(./static/assets/images/splash-page2.svg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
</style>

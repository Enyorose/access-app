<template>
  <div class="splash">
    <Header :pageInfo="pageInfo" />
    <article>
      <h1>A Future of Accessibilities...</h1>
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

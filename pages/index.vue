<template>
  <div class="splash">
    <Header />
    <article>
      <h1>
      A Future of Accessibilities...
      </h1>

    </article>
    <Footer />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
h1{
  font-size: 5em;
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

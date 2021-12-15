<template>
 
  <div>
    <div class="flex justify-between align-center p-5">
      <Header />
      <Nav />
      
    </div>
    <Community />
  </div>
  

</template>
<script>
export default {
  data() {
    return {
      pageInfo: {
        menuName: "community",
        header: "Community",
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
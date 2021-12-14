<template>
  <main>
    <div>
      <Header :pageInfo="pageInfo" />
    </div>
    <Community />
  </main>
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

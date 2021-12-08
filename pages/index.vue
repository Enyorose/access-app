<template>
  <div>
    <Footer :footerInfo="groupInfo" />
  </div>
</template>

<script>
export default {
  data () {
    return {
      groupInfo: {
        name: 'VeBuWa Group',
        year: '2021',
        license: 'MIT License'
      }
    }
  }
    
};
</script>

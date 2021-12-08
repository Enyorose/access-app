<template>
  <div>
    <p>&copy; {{ footerInfo.name }} {{ footerInfo.year }} | {{ footerInfo.license }} </p>
  </div>
</template>
<!-- JS -->
<script>
export default {
  props: ['footerInfo']
}
</script>
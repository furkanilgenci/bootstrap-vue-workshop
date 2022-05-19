<template lang="pug">
.card-container
  h3 {{ name }}
  p {{ description }}
  button.btn.btn-primary Rent

</template>

<script>
export default {
  name: 'CarCard',
  props: {
    name: String,
    description: String,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card-container {
  border: 1px solid #d0d0d0;
  padding: 12px;
  margin-bottom: 24px;
  border-radius: 8px;
}
</style>

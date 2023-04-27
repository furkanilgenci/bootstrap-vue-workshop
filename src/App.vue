<script setup>
</script>

<template>
  <div>
    <h1>hello</h1>
    <button class="btn btn-primary">Primary button</button>
    <button class="btn btn-secondary">Secondary button</button>

  </div>
  
</template>

<style scoped>
nav {
  width: 100%;
  font-size: 12px;
  margin-top: 2rem;
  position: absolute;
  top: 0;
  right: 0;
  display: flex;
  justify-content: flex-end;
  gap: 1rem;
  font-size: 1rem;
  padding: 1rem 0;
}
.logo {
  margin: 0 2rem 0 0;
}
.projects {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}
</style>
<template>
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<script>
  export default {
    props: ['title'],
  }
</script>

<style scoped>
  header {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 5rem;
    border-radius: 5px;
    background-color: #ED6A5E;
  }

  header h1 {
    margin: 0;
    color: #fff;
  }
</style>

<template>
  <the-header title="Remember Me"></the-header>
  <the-resources></the-resources>
</template>

<script>
  import TheHeader from './components/layout/TheHeader.vue';
  import TheResources from './components/learning-resources/TheResources.vue';

  export default {
    components: {
      TheHeader,
      TheResources,
    },
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Commissioner:wght@400;500&family=Forum&family=Open+Sans:wght@400;500;700&family=Roboto&display=swap');

  *{
    box-sizing: border-box;
  }

  *::after,
  *::before {
    box-sizing: inherit;
  }

  body {
    margin: auto;
    padding: 0 25px;
    font-family: 'Roboto', sans-serif;
  }
</style>

<template>
  <stored-resource :resources="storedResources"></stored-resource>
</template>

<script>
  import StoredResource from './components/learning-resources/StoredResources.vue';

  export default {
    components: {
      StoredResource,
    },
    data() {
      return {
        storedResources: [
          {
            id: 'official-guide',
            title: 'Official guide',
            description: 'The official Vue.js docs',
            link: 'https://vuejs.org',
          },
          {
            id: 'google',
            title: 'Google',
            description: 'Learn to google...',
            link: 'https://google.com',
          },
        ]
      }
    }
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

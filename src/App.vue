<template>
  <ul>
    <learning-resources
    v-for="res in storedResources"
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link"
    ></learning-resources>
  </ul>
</template>

<script>
  import LearningResources from './components/learning-resources/LearningResource.vue';

  export default {
    components: {
      LearningResources,
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
    margin: 0;
    font-family: 'Roboto', sans-serif;
  }
</style>

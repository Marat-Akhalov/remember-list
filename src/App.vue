<template>
  <ul></ul>
</template>

<script>
  export default {
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

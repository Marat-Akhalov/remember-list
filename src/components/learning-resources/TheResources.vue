<template>
  <base-card>
    <base-button @click="setSelectedTab('stored-resources')">Stored Resources</base-button>
    <base-button @click="setSelectedTab('add-resource')">Add Recourses</base-button>
  </base-card>
  <component :is="selectedTab"></component>
</template>

<script>
import StoredResources from './StoredResources.vue';
import AddResource from './AddResource.vue';


  export default {
    components: {
      StoredResources,
      AddResource
    },
    data() {
      return {
        selectedTab: 'stored-resources',
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
    },
    provide() {
      return {
        resources: this.storedResources,
      }
    },
    methods: {
      setSelectedTab(tab) {
        this.selectedTab = tab;
      }
    }
  }
</script>

<template>
  <base-card>
    <base-button @click="setSelectedTab('stored-resources')">Stored Resources</base-button>
    <base-button @click="setSelectedTab('add-recourse')">Add Recourses</base-button>
  </base-card>
</template>

<script>
  export default {
    data() {
      return {
        selectedTab: 'stored-recourses',
      }
    },
    methods: {
      setSelectedTab(tab) {
        this.selectedTab = tab;
      }
    }
  }
</script>

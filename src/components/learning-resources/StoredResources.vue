<template>
  <ul>
    <learning-resources
    v-for="res in resources"
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link"
    :id="res.id"
    ></learning-resources>
  </ul>
</template>

<script>
import LearningResources from './LearningResource.vue';

  export default {
    components: {
      LearningResources,
    },
    inject: ['resources'],
  }
</script>

<style scoped>
  ul {
    margin: 0;
    padding: 0;
    list-style-type: none;
  }
</style>

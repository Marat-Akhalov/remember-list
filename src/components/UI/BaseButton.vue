<template>
  <button
  :type="type"
  :class="mode"
  >
    <slot></slot>
  </button>
</template>

<script>
  export default {
    props: ['type', 'mode'],
  }
</script>

<style scoped>
  button {
    padding: 75rem 1.5rem;
    border: 1px solid salmon;
    color: whitesmoke;
    background-color: #045257;
    cursor: pointer;
  }

  button:hover,
  button:active {
    border-color: blue;
    background-color: #0ea9b4;
  }

  .flat {
    border: none;
    color: #0ea9b4;
    background-color: transparent;
  }

  .flat:hover,
  .flat:active {
    background-color: palevioletred;
  }
</style>

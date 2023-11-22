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
    padding: 0.75rem 1.5rem;
    color: whitesmoke;
    background-color: #377771;
    cursor: pointer;
  }

  button:hover,
  button:active {
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

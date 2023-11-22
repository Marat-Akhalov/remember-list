<template>
  <li>
    <base-card>
      <header>
        <h3>{{ title }}</h3>
        <base-button>Delete</base-button>
      </header>
      <p>{{ description }}</p>
      <nav>
        <a :href="link">View Resource</a>
      </nav>
  </base-card>
  </li>
</template>

<script>
  export default {
    props: ['title', 'description', 'link'],
  }
</script>

<style scoped>
  header {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  a {
    text-decoration: none;
    color: #FF8E72;
  }

  button {
    padding: 0.25rem 0.5rem;
    border: 1px solid #377771;
    border-radius: 4px;
    font-size: 14px;
    font-weight: bold;
    color: #000;
    background-color: #4ce0b3;
    cursor: pointer;
  }
</style>

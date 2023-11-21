<template>
  <li>
    <div>
      <header>
        <h3>{{ title }}</h3>
        <button>Delete</button>
      </header>
    </div>
    <p>{{ description }}</p>
    <nav>
      <a :href="link">View Resource</a>
    </nav>
  </li>
</template>

<script>
  export default {
    props: ['title', 'description', 'link'],
  }
</script>

<style scoped>
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

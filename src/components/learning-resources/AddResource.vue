<template>
  <base-card>
    <form>
      <div class="form-control">
        <label for="title">Title</label>
        <input id="title" name="title" type="text" ref="titleInput">
      </div>
      <div class="form-control">
        <label for="description">Description</label>
        <textarea id="description" name="description" rows="3" ref="descriptionInput"></textarea>
      </div>
      <div class="form-control">
        <label for="link">Link</label>
        <input id="link" name="link" type="url" ref="linkInput">
      </div>
      <div>
        <base-button type="submit">Add Resource</base-button>
      </div>
    </form>
  </base-card>
</template>

<script>
  export default {
    inject: ['addResources'],
    methods: {
      submitData() {
        const enteredTitle = this.$refs.titleInput.value;
        const enteredDescription = this.$refs.descriptionInput.value;
        const enteredLink = this.$refs.linkInput.value;
      }
    }
  }
</script>

<style scoped>
  label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: bold;
  }

  input,
  textarea {
    display: block;
    width: 100%;
    padding: 0.15rem;
    border: 1px solid #ccc;
    font: inherit;
  }

  input:focus,
  textarea:focus {
    border-color: #ed6a5e;
    outline: none;
    background-color: rgba(14, 169, 180, 0.2);
  }

  .form-control {
    margin: 1rem 0;
  }
</style>

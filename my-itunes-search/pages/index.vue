<template>
  <div class="container">
    <h1>Search iTunes</h1>

    <form @submit.prevent="submit">
      <input v-model="search" placeholder="Enter Artist Name" autofocus />
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      search: ''
    }
  },
  methods: {
    submit(event) {
      this.$router.push(`results/${this.search}`)
    }
  }
}
</script>

<style>
* {
  text-align: center;
}

h1 {
  padding: 20px;
}
</style>

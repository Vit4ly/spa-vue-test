<template>
<div>
  <h1>List</h1>

  <hr>
  <table v-if="tasks.length">

  </table>
<p v-else>No Tasks</p>
</div>
</template>

<script>
export default {
  name: "List.vue",
  computed: {
    tasks() {
      return this.$store.getters.tasks
    }
  }
}
</script>

<style scoped>

</style>

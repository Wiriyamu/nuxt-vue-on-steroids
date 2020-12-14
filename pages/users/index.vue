<template>
  <div>
    <h1>The users View</h1>
    <input
      v-model.number="userId"
      style="border: 1px solid black"
      type="text"
    />
    <button
      style="padding: 5px 10px; background-color: blue; color: white"
      @click="onLoadUser"
    >
      Load User
    </button>
  </div>
</template>

<script>
export default {
  name: 'Users',
  data: () => ({
    userId: null,
  }),

  methods: {
    onLoadUser() {
      this.$router.push(`/users/${this.userId}`)
    },
  },
}
</script>

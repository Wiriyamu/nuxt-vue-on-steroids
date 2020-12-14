<template>
  <header>
    <h1>Nuxt App</h1>
    <ul style="list-style: none">
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/users">Users</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  background-color: white;
  padding: 1% 1%;
}

ul {
  display: flex;
}
li {
  padding-right: 10px;
}
</style>

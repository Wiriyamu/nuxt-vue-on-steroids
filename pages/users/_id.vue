<template>
  <h1>A single user: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  name: 'Id',
  layout: 'users',
  // Validate Method (https://pt.nuxtjs.org/docs/2.x/components-glossary/pages-validate)
  validate({ params }) {
    return /^\d+$/.test(params.id)
  },
}
</script>

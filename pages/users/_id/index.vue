<template>
  <span>Hey {{ $route.params.id }}</span>
</template>

<script>
export default {
  validate(data) {
    return /^\d+$/.test(data.params.id)
  },
}
</script>

<style></style>

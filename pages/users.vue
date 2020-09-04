<template>
  <span>
    <v-text-field v-model="id" label="Textfield" solo></v-text-field>
    <v-btn @click="goId()">Submit</v-btn>
    <nuxt-child />
  </span>
</template>

<script>
export default {
  data: () => {
    return {
      id: '',
    }
  },
  methods: {
    goId() {
      this.$router.push('/users/' + this.id)
    },
  },
  layout: 'users',
}
</script>

<style></style>

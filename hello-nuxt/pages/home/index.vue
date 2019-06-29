<template>
  <div>
    <h2>Home page</h2>
    <button @click="sayHello">say Hello</button>
  </div>
</template>

<script>
export default {
  methods: {
    sayHello() {
      this.$debug('say hello!!!')
    }
  }
}
</script>

<style scoped>

</style>



<template>
  <div>
    <p v-if="showMessage">Message Showed</p>
    <p v-else>Message</p>
    <button v-on:click="changeValue">change value show msg</button>
  </div>
</template>

<script>
export default {
  name: "IfElse",
  data() {
    return {
      showMessage: true
    }
  },
  methods: {
    changeValue(){
      this.showMessage = !this.showMessage
    }
  }
}
</script>

<style scoped>

</style>

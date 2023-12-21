<template>
  <h6 v-bind:class="{ red: classRed}">h7h6h6h6</h6>
  <button v-on:click="changeColor">click</button>
</template>

<script>
  export default{
    name: "dinamic-class",
    data() {
      return {
        classRed: true,
      };
    },
    methods: {
      changeColor(){
        this.classRed = !this.classRed
      }
    }
  }
</script>

<style scoped>
  .red{
    background: red;
  }
</style>
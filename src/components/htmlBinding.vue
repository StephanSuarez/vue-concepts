<template>
  <p v-html="ej"></p>
  <div v-html="ej2"></div>
</template>

<script>
  export default{
    name: "htmlBinding",
    data() {
      return {
        ej: 'this is ',
        ej2: "<p>p p p p p p p p p p p p</p>"
      }
    }
  }
</script>

<style></style>
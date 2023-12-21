<template>
  <div>
    <p>{{ typeof message }}</p>
    <p>{{ message }}</p>
    <p>{{ typeof data }}</p>
    <p>{{ data }}</p>
  </div>
</template>

<script>
  export default{
    name: "MyInterpolation",
    data() {
      return{
        message: "Message",
        data: {
          name: "Data Name",
          age: 123,
          array: [1, 2, 3, 'a', 'b'],
          obj: {
            again: 'again'
          }
        }
      }
    }
  }
</script>

<style>

</style>
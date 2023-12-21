<template>
  <h6>Click on the btn to get the name</h6>,
  <button v-on:click="getUser(name)">click</button>
  <button v-on:click="num = getNum(5, 2)">click get num</button>
  <p v-html="num"></p>
</template>

<script>
  export default{
    name: "child-father-t",
    data() { 
      return {
        name: "stephan",
        num: ''
      }
    },
    props:{
      nnn: String,
      getUser: Function,
      getNum: Function,
    }
  }
</script>

<style></style>
<template>
  <div>
    <p>Message: {{ msgUpper }}</p>
    <p>Message: {{ msgUpperMethod() }}</p>
    <p>Number To Zero: {{ numberToZero }} </p>
  </div>
</template>

<script>
  export default{
    name: 'computed-property',
    data() {
      return {
        msg: 'hello'
      }
    },
    props: {
      number: Number
    },
    computed: {
      msgUpper(){
        return this.msg.toUpperCase();
      },
      numberToZero(){
        if(typeof this.number == 'number'){
          return this.number*0
        }
        return "Dont have a number"
      }
    },
    methods:{
      msgUpperMethod(){
        return this.msg.toUpperCase();
      }
    }
  }
</script>

<style></style>
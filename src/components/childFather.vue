<template>
  <h6>Sending data Father to Child</h6>
  <childFatherT :get-user="getUserName" :nnn="hol" :get-num="getNum"/>
</template>

<script>
import childFatherT from './childFather2.vue';

  export default{
    name: "child-father",
    data() { 
      return {
        je: "fals;d"
      }
    },
    methods:{
      getUserName(name) {
        alert(name)
      },
      getNum(n1, n2){
        let result = n1+n2;
        return ("", n1, "+", n2, "=", result)
      }
    },
    components: {
      childFatherT
    }
  }
</script>

<style></style>